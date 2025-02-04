# 🦙📚 Demonstration chatbot with Streamlit, LlamaIndex and Google Gemini

Build a chatbot hosted on Streamlit Community Cloud and powered by LlamaIndex that augments Google Gemini with local documents. This repository is used in the Build Your Own AI Chatbot offered by <a href="https://library.sjsu.edu/digitalhumanities">King Library's Digital Humanities Center</a>. The original code for this chatbot is based on the chabtot described in <a href="https://blog.streamlit.io/build-a-chatbot-with-custom-data-sources-powered-by-llamaindex/">this blog post.</a>

The demo chatbot is an expert on the works of author Rabindranath Tagore. Fork the repository and add your own documents to create a chatbot that focuses on a different topic.

## Overview of the App

<img src="app-image-25.png" width="75%">

- Takes user queries via Streamlit's `st.chat_input` and displays both user queries and model responses with `st.chat_message`
- Uses LlamaIndex to load and index data and create a chat engine that will retrieve context from that data to respond to each user query

## Demo App

<a href="https://sjsu-chatbot-workshop.streamlit.app/">https://sjsu-chatbot-workshop.streamlit.app/</a>

## Build your own copy

Follow the steps in the workshop slides at <a href="https://tiny.sjsu.edu/chatbot-workshop">https://tiny.sjsu.edu/chatbot-workshop</a>

> [!CAUTION]
> Don't commit your secrets file to your GitHub repository. The `.gitignore` file in this repo includes `.streamlit/secrets.toml` and `secrets.toml`. 

## Try out the app

Once the app is loaded, enter your question about Rabindranath Tagore and wait for a response.

## Source texts

The demo version of the chatbot uses texts from the writer <a href="https://www.nobelprize.org/prizes/literature/1913/tagore/biographical/">Rabindranath Tagore</a>. These texts are available from <a href="https://www.gutenberg.org/ebooks/search/?query=tagore&submit_search=Go%21"> Project Gutenberg</a>.
