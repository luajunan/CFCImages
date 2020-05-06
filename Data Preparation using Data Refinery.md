# COVID Crisis Communications Starter Kit


## Chapter 1 Introduction

This workshop is an introduction to Watson Studio, the IBM platform for data science and artificial intelligence. Completing the exercises does not require any specific skills or knowledge. At the end of this session you should be able to use the product on your own.

In this workshop, we will:

    Setup your Watson Studio Cloud account

    Prepare data using Data Refinery

    Build and Deploy models in Jupyter Notebooks to detect fraud

    Create a model using AutoAI

    Create a model using the SPSS canvas

To begin, please clone the relevant data files that would be the baseline for to following workshop exercises.

FILES TO GITHUB


## Authors

- [Donna Byron](https://developer.ibm.com/profiles/dkbyron/) - IBM
- [John Walicki](https://developer.ibm.com/profiles/walicki/) - IBM
- [Matt Price](https://developer.ibm.com/profiles/pricem/) - IBM
- [Mofizur Rahman](https://developer.ibm.com/profiles/mofizur.rahman) - IBM
- [Pooja Mistry](https://developer.ibm.com/profiles/pmistry/) - IBM
- [Upkar Lidder](https://developer.ibm.com/profiles/ulidder/) - IBM

## Contents

1. [Overview](#overview)
2. [Video](#video)
3. [The idea](#the-idea)
4. [How it works](#how-it-works)
5. [Diagrams](#diagrams)
6. [Documents](#documents)
7. [Datasets](#datasets)
8. [Technology](#technology)
9. [Getting started](#getting-started)
9. [Resources](#resources)
10.[License](#license)

## Overview

<p align="center">
<img width="50%" height="50%" src="https://raw.githubusercontent.com/Call-for-Code/Solution-Starter-Kit-Communication-2020/master/starter-kit/assistant/WA-Photo101.png">
</p>


### Connect your chatbot to data sources via a webhook

Now that you’ve created your Watson Assistant-enabled chatbot, you need to connect it to a data source. With Watson Assistant, you need to do this via a webhook.

A webhook is a mechanism that allows you to call out to an external program based on something happening in your program. When used in a dialog skill, a webhook is triggered when the assistant processes a node that has a webhook enabled. The webhook collects data that you specify or that you collect from the user during the conversation and save in context variables. It sends the data as part of a HTTP POST request to the URL that you specify as part of your webhook definition. The URL that receives the webhook is the listener. It performs a predefined action using the information that you pass to it as specified in the webhook definition, and can optionally return a response.

[Follow these instructions for setting up webhook](./starter-kit/webhook/README.md) with the Watson Assistant chatbot you just provisioned.

### Integrate your COVID-19 chatbot with Slack

Now that you have a functioning Watson Assistant, let's deploy it to Slack. Slack is a cloud-based messaging application that helps people collaborate with one another. After you configure a dialog skill and add it to an assistant, you can integrate the assistant with Slack.

When integrated, depending on the events that you configure the assistant to support, your assistant can respond to questions that are asked in direct messages or in channels where the assistant is directly mentioned.

[Read these instructions](/starter-kit/slack/README.md) to learn how to integrate your COVID-19 chatbot with Slack.

![Slack Gif](/starter-kit/slack/readme_images/Slack.gif)

### Integrate your COVID-19 chatbot with Node-RED

Want to create a voice-enabled chatbot? This tutorial teaches you how to [create a voice enabled chatbot using Node-RED](./starter-kit/node-red/README.md) and the Watson Assistant, Watson Speech to Text, and Watson Text to Speech nodes.

### Embed your COVID-19 chatbot on a Node.js website

Finally, you can embed your COVID-19 crisis communication chatbot on a Node.js website.

- Follow the [COVID-Simple installation instructions](./starter-kit/covid-simple/README.md)

## Disclosures

This tool is intended to provide information based on currently available CDC and other public information to help you make decisions about seeking appropriate medical care. This system is not intended for the diagnosis or treatment of disease or other conditions, including COVID-19, and you should not provide any personally identifying or private health information.

This Watson Assistant bot is populated with data that is sourced from the following resources:

- Most static responses provide information found on the CDC's COVID FAQ Page: https://www.cdc.gov/coronavirus/2019-ncov/faq.html
- Dynamic infection and death counts are sourced from Johns Hopkins University via the following API: https://www.covid19api.com/
- Dynamic news stories are sourced from Watson Discovery's news feed. Additional information on that service can be found here: https://www.ibm.com/watson/services/discovery-news/

## License

This solution starter is made available under the [Apache 2 License](LICENSE).
