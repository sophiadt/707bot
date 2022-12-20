# 707 Discord AI Chat Bot

An AI discord bot that can simulate a conversation with RFA's best hacker, 707 from [Mystic Messenger](https://en.wikipedia.org/wiki/Mystic_Messenger)!

Credits to Lynn Zheng and her [Discord AI Chatbot tutorial](https://www.freecodecamp.org/news/discord-ai-chatbot/) for helping me build this.

The chatbot uses the [Microsoft DialoGPT conversational model](https://huggingface.co/microsoft/DialoGPT-medium) that has been trained with [707's messages in the Deep Story from this Kaggle dataset](https://www.kaggle.com/datasets/pineapplesoup/707-messages). The dataset has almost 4000 lines and I trained it for 12 epochs to give a perplexity of around 1.3. The perplexity represents how confused the model is so the higher the perplexity, the more confused the model is. 1.3 is a very low perplexity but the chat bot still has some out-of-character responses. With this amount of data, the model took around 1.5 hours to train.

If you want to try out my chatbot, you can go [here](https://huggingface.co/sophiadt/DialoGPT-medium-707?text=Hi%21+I%27m+MC%7E) where it's hosted on Hugging Face's Model Hub.

## Project Files

* `model_train_upload_workflow.ipyb`: Notebook to be run in Google Colab to train and upload the model to Hugging Face's Model Hub
* `main.py`: Script to be imported into a Repl.it Python Discord.py project
* `keep_alive.py`: Script to keep the discord bot alive for half an hour after main.py is run

## Resource Links
* [Lynn Zheng's tutorial on freeCodeCamp](https://www.freecodecamp.org/news/discord-ai-chatbot/)
* [Lynn Zheng's video tutorial on YouTube](https://youtu.be/UBwvFuTC1ZE)
* [707 messages dataset on Kaggle](https://www.kaggle.com/datasets/pineapplesoup/707-messages)
* [My Hugging Face Model](https://huggingface.co/sophiadt/DialoGPT-medium-707)
