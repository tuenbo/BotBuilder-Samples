# Console EchoBot
Bot Framework v4 console echo sample.

This bot has been created using [Bot Framework](https://dev.botframework.com), it shows how to create a simple bot that you can talk to from the console window.

This sample shows a simple echo bot and demonstrates the bot working as a console app using a sample console adapter.

## To try this sample
- Clone the repository
```bash
git clone https://github.com/Microsoft/botbuilder-samples.git
```
- Bring up a terminal, navigate to `botbuilder-samples\samples\python\01.console-echo` folder
- In the terminal, type `pip install -r requirements.txt`
- type 'python main.py'


# Adapters
[Adapters](https://docs.microsoft.com/azure/bot-service/bot-builder-concept-activity-processing?view=azure-bot-service-4.0#the-bot-adapter) provide an abstraction for your bot to work with a variety of environments. 

A bot is directed by it's adapter, which can be thought of as the conductor for your bot. The adapter is responsible for directing incoming and outgoing communication, authentication, and so on. The adapter differs based on it's environment (the adapter internally works differently locally versus on Azure) but in each instance it achieves the same goal. 

In most situations we don't work with the adapter directly, such as when creating a bot from a template, but it's good to know it's there and what it does.
The bot adapter encapsulates authentication processes and sends activities to and receives activities from the Bot Connector Service. When your bot receives an activity, the adapter wraps up everything about that activity, creates a [context object](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-activity-processing?view=azure-bot-service-4.0#turn-context), passes it to your bot's application logic, and sends responses generated by your bot back to the user's channel.


# Further reading

- [Bot basics](https://docs.microsoft.com/azure/bot-service/bot-builder-basics?view=azure-bot-service-4.0)
- [Channels and Bot Connector service](https://docs.microsoft.com/azure/bot-service/bot-concepts?view=azure-bot-service-4.0)
- [Activity processing](https://docs.microsoft.com/azure/bot-service/bot-builder-concept-activity-processing?view=azure-bot-service-4.0)