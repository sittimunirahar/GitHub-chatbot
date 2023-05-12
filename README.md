# GitHub Chatbot - Custom Question Answering

This is an Azure Bot Framework called GitHub Chatbot. It is a custom question answering bot that uses a trained knowledge base as its source. The sources were generated from Github Documentation of Get Started https://docs.github.com/en/get-started, editorial and chit chat. 

This bot framework SDK source code is generated from Azure bot created in my azure subscription. 

This project is for [Microsoft Code; Without Barriers Hackathon 2023](https://cwb2023.devpost.com/)

## Concepts implemented

In this bot, several features are demonstrated:
1. Active learning
2. Follow-up prompts (multiturn conversation)
3. User interface design: hero card and suggestion card
4. Question answering 
5. Friendly chit chat

## Prerequisites

1. Create azure subscription 
2. Create language resource with custom question answering enabled
3. Create and deploy knowledge base in Language Studio
    * Import file
4. Clone this bot framework SDK source code
5. Provision and publish the bot
    * https://learn.microsoft.com/en-us/azure/bot-service/provision-and-publish-a-bot?view=azure-bot-service-4.0&tabs=userassigned%2Ccsharp
6. Test bot in web chat

## Trying out the chatbot

### Hero card & multi-turn prompt:

Click on ‘Quickstart’ or any option on Welcome message prompt

### Suggestion card:

After getting atleast one answer, click on ‘Glossary’ on suggestion card at the bottom of the chat

### Question Answering:

Type ‘What is GitHub?’

### Friendly chit chat:

Type ‘How are you?’

### Active learning:

1. Enter ambiguous utterance: ‘create a repo’
2. Notice that the bot returns 'Did you mean?' with a few suggestions
3. 

