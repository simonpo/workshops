# Workshop 4: Cognitive Services & Bot Framework

## Introduction

Before the team can begin working on Cognitive Services and Bot Framework tasks, everyone needs to have a development environment set up with approriate tools. This workshop will get you ready to begin developing Bots, and includes hands-on experience with the following elements:

*Bot Framework
*QnAMaker
*LUIS
*Speech & Text analytics, translation
*Deployment
*Using PowerBI to visualize results

## Required Software

*[VS Code](https://code.visualstudio.com/Download)
*[Bot Framework Emulator](https://github.com/Microsoft/BotFramework-Emulator)

## Account Setup
*[QnA Maker Account](https://www.qnamaker.ai/)
*[Text Analytics API](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-signup)

## VS Code

Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity). There are many extensions for Azure services available via Visual Studio Code.

## Bot Framework Emulator

The [Bot Framework Emulator](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-debug-emulator?view=azure-bot-service-4.0) is a desktop application that allows bot developers to test and debug their bots, either locally or remotely. Using the emulator, you can chat with your bot and inspect the messages that your bot sends and receives. The emulator displays messages as they would appear in a web chat UI and logs JSON requests and responses as you exchange messages with your bot. Before you deploy your bot to the cloud, run it locally and test it using the emulator. You can test your bot using the emulator even if you have not yet created it with Azure Bot Service or configured it to run on any channels.

## Azure Bot Service

Azure Bot Service provides an integrated environment that is purpose-built for bot development, enabling you to build, connect, test, deploy, and manage intelligent bots, all from one place. Azure Bot Service leverages the Bot Builder SDK with support for C# and JavaScript.

Your bot is a web service that implements a conversational interface and communicates with the Bot Framework Service to send and receive messages and events. You can create bots in any number of environments and languages. You can start your bot development in the Azure portal, or use [C# | JavaScript] templates for local development.

As part of the Azure Bot Service, we offer additional components you can use to extend your bot's functionality

### Add natural language processing
Enable your bot to understand natural language, understand spelling errors, use speech, and recognize the user's intent

### How to use LUIS
Add a knowledge base to answer questions users ask in a more natural, conversational way
How to use QnA Maker

### Manage multiple models
If using more than one model, such as for LUIS and QnA Maker, intelligently determine when to use which one during your bot's conversation
Dispatch tool

### Add cards and buttons
Enhance the user experience with media other than text, such as graphics, menus, and cards
How to add cards

### Testing
Test your bot locally with the emulator. The Bot Framework Emulator is a stand-alone app that not only provides a chat interface, but also debugging and interrogation tools to help understand how and why your bot does what it does. The emulator can be run on a locally alongside your in-development bot application.

Test your bot on the web. Once configured through the Azure portal your bot can also be reached through a web chat interface. The web chat interface is a great way to grant access to your bot to testers and other people who do not have direct access to the bot's running code.

## QnAMaker

You can use [QnA Maker service](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-howto-qna?view=azure-bot-service-4.0&tabs=cs) to add question and answer support to your bot. One of the basic requirements in creating your own QnA Maker service is to seed it with questions and answers. In many cases, the questions and answers already exist in content like FAQs or other documentation. Other times you would like to customize your answers to questions in a more natural, conversational way.

## LUIS

The ability to understand what your user means conversationally and contextually can be a difficult task, but can provide your bot a more natural conversation feel. Language Understanding, called [LUIS](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-howto-v4-luis?view=azure-bot-service-4.0&tabs=cs), enables you to do just that so that your bot can recognize the intent of user messages, allow for more natural language from your user, and better direct the conversation flow.

## Speech & Text Analytics 
The [Text Analytics API](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/overview) is a cloud-based service that provides advanced natural language processing over raw text, and includes four main functions: sentiment analysis, key phrase extraction, language detection, and entity linking.

*[Sentiment Analysis](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-sentiment-analysis)
Analyze raw text for clues about positive or negative sentiment. This API returns a sentiment score between 0 and 1 for each document, where 1 is the most positive.

The analysis models are pretrained using an extensive body of text and natural language technologies from Microsoft. For selected languages, the API can analyze and score any raw text that you provide, directly returning results to the calling application.

*[Key Phrase Extraction](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-keyword-extraction)
Automatically extract key phrases to quickly identify the main points. For example, for the input text "The food was delicious and there were wonderful staff", the API returns the main talking points: "food" and "wonderful staff".

*[Language Detection](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-language-detection)
For up to 120 languages, detect which language the input text is written in and report a single language code for every document submitted on the request. The language code is paired with a score indicating the strength of the score.

*[Entity Recognition (Preview)](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/how-tos/text-analytics-how-to-entity-linking)
Identify and categorize entities in your text as people, places, organizations, date/time, quantities, percentages, currencies, and more. Well-known entities are also recognized and linked to more information on the web.
REST

## Deployment

## Using PowerBI to vizualize results

placeholder
