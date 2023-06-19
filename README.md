# GitHub Chatbot - Custom Question Answering

🤖 This is an Azure Bot called GitHub Chatbot. It is a custom question answering bot that uses a trained knowledge base as its source, generated from Github Documentation of Get Started https://docs.github.com/en/get-started, editorial and chit chat. 

Built with: Azure bot framework sdk, Azure language studio, Netlify, node.js, vscode

This project is for [Microsoft Code; Without Barriers Hackathon 2023](https://cwb2023.devpost.com/)
Project submission can be found here: https://devpost.com/software/github-chatbot

The project won third place 🎉 under Github problem statement 

## Concepts implemented

In this bot, several features are demonstrated:
1. Active learning
2. Follow-up prompts (multiturn conversation)
3. UI design for bot: hero card and suggestion card
4. Question answering 
5. Friendly chit chat

## Prerequisites

1. Create azure subscription 
2. Create language resource with custom question answering enabled
3. Create and deploy knowledge base in Language Studio
    1. Download githubqna_qnas.xlsx in public folder
    2. Open language studio, sign in and select resource (the language resources created previously in Azure portal)
    3. Create new > custom question answering
    4. Manage sources > add source > file
    5. Add file
    6. Enter source name, choose file
    7. Add all
    8. Upon completion, verify that the sources list now has chitchat friendly, Open source, Get started and editorial
    9. Edit knowledge base accordingly
    10. Deploy knowledge base > Deploy
4. Clone this bot framework SDK source code
5. Provision and publish the bot by following the instructions below:
    * https://learn.microsoft.com/en-us/azure/bot-service/provision-and-publish-a-bot?view=azure-bot-service-4.0&tabs=userassigned%2Ccsharp
6. Test bot in web chat

## Trying out the chatbot

### Hero card & multi-turn prompt:

Click on ‘Quickstart’ or any option on Welcome message prompt

The bot should return a respond with multiple choices

### Suggestion card:

After getting atleast an answer from the bot, a suggestion card should persistently appear at the bottom of the bot
click any of the button 

The bot should return the appropriate respond

### Question Answering:

Type ‘What is GitHub?’

The bot should return an answer that describes about GitHub

### Friendly chit chat:

Type ‘How are you?’

The bot should return a friendly respond

### Active learning:

1. Enter ambiguous utterance: ‘create a repo’
2. Notice that the bot returns 'Did you mean?' with a few suggestions
3. Click one of the options
4. Open language studio, 

