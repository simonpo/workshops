# Workshop 4: Cognitive Services & Bot Framework

## Introduction

This workshop will begin with creating a Node.js bot in the Azure portal. We will discuss the basics of a bot and how to use Azure Bot Service with LUIS (Language Understanding Intelligent Service). We will also learn how to visualize app analytics in Power Bi. For the first part of the workshop you only need to be logged into your Azure portal and luis.ai. 

The second part of this workshop will show you how to deploy a java bot into the Azure portal. 

The last part of the workshop will demo Cognitive Services APIs and walk through how to create a FAQ bot using QnA Maker. 

This workshop will get you ready to begin developing Bots, and includes hands-on experience with the following elements:

* Bot Framework
* QnAMaker
* LUIS
* Cognitive Services
* Deployment
* Visualizing Analytics in Power Bi

## Account Setup
* [QnA Maker Account](https://www.qnamaker.ai/)
* [LUIS](https://www.luis.ai/)

## Optional Software

If you want to test the bot, continue developing the bot locally after the workshop or create a new bot locally, you need the below installed. See the bot-demo folder README for the full walkthrough of a node.js bot. For workshop purposes we will be using the Azure portal to create the bot.

* [VS Code](https://code.visualstudio.com/Download)
* [Bot Framework Emulator](https://github.com/Microsoft/BotFramework-Emulator)

## VS Code

Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity). There are many extensions for Azure services available via Visual Studio Code.

## Bot Framework Emulator

The [Bot Framework Emulator](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-debug-emulator?view=azure-bot-service-4.0) is a desktop application that allows bot developers to test and debug their bots, either locally or remotely. Using the emulator, you can chat with your bot and inspect the messages that your bot sends and receives. The emulator displays messages as they would appear in a web chat UI and logs JSON requests and responses as you exchange messages with your bot. Before you deploy your bot to the cloud, run it locally and test it using the emulator. You can test your bot using the emulator even if you have not yet created it with Azure Bot Service or configured it to run on any channels.

## Azure Bot Service

Please go to the [walkthrough here](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-quickstart?view=azure-bot-service-4.0) for the workshop demo on building a Node.js and LUIS bot in Azure Bot Services.

Azure Bot Service provides an integrated environment that is purpose-built for bot development, enabling you to build, connect, test, deploy, and manage intelligent bots, all from one place. Azure Bot Service leverages the Bot Builder SDK with support for C# and JavaScript.

Your bot is a web service that implements a conversational interface and communicates with the Bot Framework Service to send and receive messages and events. You can create bots in any number of environments and languages. You can start your bot development in the Azure portal, or use [C# | JavaScript] templates for local development.

As part of the Azure Bot Service, we offer additional components you can use to extend your bot's functionality:

### Add natural language processing
Enable your bot to understand natural language, understand spelling errors, use speech, and recognize the user's intent

### How to use LUIS
Add a knowledge base to answer questions users ask in a more natural, conversational way

### Manage multiple models
If using more than one model, such as for LUIS and QnA Maker, intelligently determine when to use which one during your bot's conversation using the Dispatch tool.

### Add cards and buttons
Enhance the user experience with media other than text, such as graphics, menus, and cards.

### Testing
Test your bot locally with the emulator. The Bot Framework Emulator is a stand-alone app that not only provides a chat interface, but also debugging and interrogation tools to help understand how and why your bot does what it does. The emulator can be run on a locally alongside your in-development bot application.

Test your bot on the web. Once configured through the Azure portal your bot can also be reached through a web chat interface. The web chat interface is a great way to grant access to your bot to testers and other people who do not have direct access to the bot's running code.

### Learn more about bot concepts and the SDK

* [See full documentation for designing, developing, testing, deploying & more](https://docs.microsoft.com/en-us/azure/bot-service/?view=azure-bot-service-4.0)
* [Understanding how bots work](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-basics?view=azure-bot-service-4.0&tabs=cs)
* [Dialogs](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-dialog?view=azure-bot-service-4.0)
* [Middleware](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-middleware?view=azure-bot-service-4.0)
* [Welcoming the user](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-welcome-user?view=azure-bot-service-4.0)
* [Principles of bot design](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-design-principles?view=azure-bot-service-4.0)
* [Connecting a bot to channels](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-manage-channels?view=azure-bot-service-4.0)
* [.NET SDK](https://github.com/Microsoft/botbuilder-dotnet)
* [JavaScript SDK](https://github.com/Microsoft/botbuilder-js)

## QnAMaker

You can use [QnA Maker service](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-howto-qna?view=azure-bot-service-4.0&tabs=cs) to add question and answer support to your bot. One of the basic requirements in creating your own QnA Maker service is to seed it with questions and answers. In many cases, the questions and answers already exist in content like FAQs or other documentation. Other times you would like to customize your answers to questions in a more natural, conversational way.

## LUIS

The ability to understand what your user means conversationally and contextually can be a difficult task, but can provide your bot a more natural conversation feel. Language Understanding, called [LUIS](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-howto-v4-luis?view=azure-bot-service-4.0&tabs=cs), enables you to do just that so that your bot can recognize the intent of user messages, allow for more natural language from your user, and better direct the conversation flow.

## Cognitive Services

Azure Cognitive Services are APIs, SDKs, and services available to help developers build intelligent applications without having direct AI or data science skills or knowledge. Azure Cognitive Services expand on Microsoft’s evolving portfolio of machine learning APIs and enable developers to easily add cognitive features – such as emotion and video detection; facial, speech, and vision recognition; and speech and language understanding – into their applications. The goal of Azure Cognitive Services is to help developers create applications that can see, hear, speak, understand, and even begin to reason. The catalog of services within Azure Cognitive Services can be categorized into five main pillars - Vision, Speech, Language, Search, and Knowledge.

Check out the [Cognitive Services documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/) for a full list of 5-minute quickstarts and tutorials! Or download and try out the [Intelligent Kiosk demo](https://github.com/Microsoft/Cognitive-Samples-IntelligentKiosk) where you can try out different APIs in realtime. You will need the access keys for the services in order to run the sample. See sample for more details.

* The [Text Analytics API](https://docs.microsoft.com/en-us/azure/cognitive-services/text-analytics/overview) is a cloud-based service that provides advanced natural language processing over raw text, and includes four main functions: sentiment analysis, key phrase extraction, language detection, and entity linking.

* [Face API](https://docs.microsoft.com/en-us/azure/cognitive-services/face/overview)
The Face API service is a cloud-based service that provides algorithms for analyzing human faces in images and video. The Face API has two main functions: face detection with attributes and face recognition.

* [Computer Vision API](https://docs.microsoft.com/en-us/azure/cognitive-services/computer-vision/home)
The cloud-based Computer Vision service provides developers with access to advanced algorithms for processing images and returning information. Computer Vision works with popular image formats, such as JPEG and PNG. To analyze an image, you can either upload an image or specify an image URL. Computer Vision algorithms can analyze the content of an image in different ways, depending on the visual features you're interested in. For example, Computer Vision can determine if an image contains adult or racy content, or find all the faces in an image.

* [Bing Search API](https://azure.microsoft.com/en-us/services/cognitive-services/directory/search/)
For up to 120 languages, detect which language the input text is written in and report a single language code for every document submitted on the request. The language code is paired with a score indicating the strength of the score.

* [Bing Speech API](https://azure.microsoft.com/en-us/services/cognitive-services/speech/)
Identify and categorize entities in your text as people, places, organizations, date/time, quantities, percentages, currencies, and more. Well-known entities are also recognized and linked to more information on the web.
REST

## Visualizing Analytics in Power Bi
[Power BI](https://powerbi.microsoft.com/) is a suite of business tools that helps you analyze data and share insights. Rich dashboards are available on every device. You can combine data from many sources, including Analytics queries from Azure Application Insights.

For this example we will learn how to export analytics queries. This is the preferred method. Write any query you want and export it to Power BI. You can place this query on a dashboard, along with any other data.

First, [download Power Bi Desktop](https://powerbi.microsoft.com)

Then follow the steps here to create a query and import it into Power Bi desktop: https://docs.microsoft.com/en-us/azure/application-insights/app-insights-export-power-bi?toc=/azure/azure-monitor/toc.json

## Bot Deployment for Java
Follow along with creating a Java bot locally and deploy to Azure. Documentation TBD.
