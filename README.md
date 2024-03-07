# Express Server for Payload Handling

This Express server application listens for POST requests and logs the payload to the console. It's particularly useful for testing SNS, webhooks or similar integrations locally.

## Getting Started
These instructions will get you a copy of the server up and running on your local machine.

Prerequisites

- Node.js
- ngrok (for exposing your server publicly)

## Installing

First, install the necessary packages:

```bash
npm install express body-parser request
```

## Running the server

To start the server, run:

```bash
node your_script.js
```

The server will start on port 3001. You can modify the port in the script if needed.

## Exposing with ngrok

To expose your local server to the internet using ngrok:

```bash
ngrok http 3001
```

## Usage
Send a POST request to the server endpoint (local or ngrok URL). The server will log the payload to the console. It handles AWS SNS SubscriptionConfirmation by sending a request to the SubscribeURL.