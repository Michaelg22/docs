# Slack

This guide contains information to set up a Slack Sink in Vanus Connect.

## Introduction

Slack is a cloud-based team collaboration platform that allows users to communicate, share files, and integrate with other tools and services.

With Slack Sink connector in Vanus Connect, you can easily forward real-time updates to a Slack group chat, allowing your team to stay up-to-date on all events generated by your application.


## Prerequisites

Before forwarding events to Slack, you must have:

- A Slack Account
- A [Vanus Cloud account](https://cloud.vanus.ai)

## Getting Started

To set up an app for receiving events in your Slack channel:

**Note: If you already have created a Slack App, you can skip Step 1 and directly go to [Step 2](#step-2-create-an-incoming-webhook).**

### Step 1: Create a Slack App
1. Create an [App on Slack](https://api.slack.com/apps).
   ![](images/1.png)
2. Select From Scratch.
   ![](images/2.png)
3. Set the app name and Workspace.
![](images/3.png)

### Step 2: Create an Incoming Webhook
1. Select **Incoming Webhooks** in the sidebar menu.
![img.png](images/4.png)
2. Turn on Webhooks and scroll down and click **Add New Webhook to Workspace** to add new webhook.
![](images/5.png)
3. Select the channel to receive messages.
![img.png](images/6.png)
4. Now copy the webhook URL.
![](images/7.png)
   
### Step 3: Set up your Connection in Vanus Connect 

1. Paste the Webhook URL into the `URL` field, and Click on submit to finish the configuration. 
![img_2.png](images/submit-slack.png) 
   
2. You've successfully created your Vanus slack sink connection.  
![](images/finish-slack-connection.png)  

## Required Data Format

The event data must be JSON format, here a simple message, example:

```json
{
  "data": {
    "subject": "Test",
    "message": "Hello Slack!:wave: This is Sink Slack!"
  }
}
```
