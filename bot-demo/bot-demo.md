# How to create a basic bot using LUIS through CLI commands

## Use the BotBuilder Generator

In a command prompt, create a folder for the bot

``` 
md luisGreeter
cd luisGreeter
```

Confirm  npm is up to date
```
npm i npm
```
Install Yeoman and BotBuilder using npm.
yo botbuilder will generate the bot framework and code base.
Make sure to choose 'javascript' and 'basic' (not echo) when prompted!

```
npm install -g yo 
npm install -g generator-botbuilder
yo botbuilder
```
The framework and code for the bot should now be created in the luisGreeter folder. 

## Deploying LUIS models
(See more details in the DEPLOYMENT.md file in luisGreeter/deploymentScripts. Walkthrough below fixes some errors that are found in DEPLOYMENT.md)

Install the CLIs for MSBot, LUIS-APIs and Ludown
```
npm i -g msbot luis-apis ludown
```
Create and configure required resources
*Note that LUIS-KEY and AZURE-SUBSCRIPTION-ID can be the same key. Find the LUIS Key under your settings at luis.ai
```
msbot clone services -n <YOUR BOT NAME> -f deploymentScripts/msbotClone --luisAuthoringKey <LUIS-KEY> --subscriptionId <AZURE-SUBSCRIPTION-ID> --location westus
```
Parse the lu files to your LUIS model
```
ludown parse toluis --in dialogs/greeting/resources/main.lu -o cognitiveModels/ --out basicBot.luis -n luisGreeter-LUIS -d 'Bot Builder V4 Basic Bot.' --verbose
```
Create a new LUIS application using the generate LUIS model and update the .bot file with the LUIS service configuration:
```
luis import application --in cognitiveModels/basicBot.luis --authoringKey <LUIS-KEY>  --msbot --endpointRegion --region westus | msbot connect luis --stdin
```

Train the LUIS model
```
msbot get luisGreeter-LUIS | luis train version --wait --stdin
```
Publish  the LUIS model 
```
msbot get luisGreeter-LUIS | luis publish version --stdin
```
Go to your luis.ai account and you will see the new LUIS model and the trained intents/entities list.

## Updating the .bot file
After deploying LUIS your .bot file may be missing key components for running the bot locally using nodejs. Copy and paste this into the services just before the luis config.
```
	  {
	      "type": "endpoint",
	      "name": "development",
	      "id": "http://localhost:3978/api/messages",
	      "appId": "",
	      "appPassword": "",
	      "endpoint": "http://localhost:3978/api/messages"
	    }
```
(It should look something like this
```  "services": [
        {
            "type": "endpoint",
            "appId": "",
            "appPassword": "",
            "endpoint": "http://localhost:3978/api/messages",
            "id": "http://localhost:3978/api/messages",
            "name": "development"
        },
        {
            "type": "luis",
            ....
            ...)
```