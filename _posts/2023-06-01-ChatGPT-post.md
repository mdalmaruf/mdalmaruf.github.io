---
title: 'Building a Medical Assistant Chatbot using ChatGPT-4 and Python'
date: 2023-06-22
permalink: /posts/2023/06/ChatGPT-post/
tags:
  - ChatGPT-4
  - Python
  - Chatbot
  - Medical Assistant
  - Gradio
  - OpenAI
---



In this tutorial, we will walk you through the process of building a Medical Assistant Chatbot utilizing ChatGPT and Python. To enhance the interaction experience, we will employ Gradio for creating an intuitive user interface.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Setting Up Your Python Environment](#setting-up-your-python-environment)
- [Acquiring OpenAI API Key](#acquiring-openai-api-key)
- [Writing the Python Script](#writing-the-python-script)
- [Running the Chatbot](#running-the-chatbot)
- [Conclusion](#conclusion)

## Prerequisites <a name="prerequisites"></a>

Before we begin, make sure that you have Python 3 installed on your machine. If not, download it from the [official Python website](https://www.python.org/downloads/) and follow the installation instructions for your operating system.

You should also create a GitHub repository to store and manage the project's code and documentation. If you are new to GitHub, you can follow this [guide](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) on creating a new repository.

## Setting Up Your Python Environment <a name="setting-up-your-python-environment"></a>

It’s a good practice to create a virtual environment for your Python project. This helps to manage dependencies efficiently.

### Creating a Virtual Environment

```sh
python -m venv chatbot-env
```
### Activate the virtual environment:

- On Windows:
  ```sh chatbot-env\Scripts\activate
  ```

- On macOS and Linux:
  ```sh source chatbot-env/bin/activate
  ```

### Installing Required Libraries
- We need to install the OpenAI library to access ChatGPT and Gradio for creating the user interface.
```sh
pip install openai gradio
```

- Gradio allows you to rapidly create web-based user interfaces for Python models. OpenAI library helps in integrating with GPT models provided by OpenAI.


## Acquiring OpenAI API Key <a name="acquiring-openai-api-key"></a>
For interacting with ChatGPT-4, you'll need an API key from OpenAI.

- Head to OpenAI and create an account.
- Once logged in, navigate to the API section to generate a new API key.
- Store the API key securely as it is needed to authenticate the requests to ChatGPT-4.
  
## Writing the Python Script <a name="writing-the-python-script"></a>
Create a Python script, named medical_chatbot.py, and write the code below:

```python
import openai
import gradio as gr

# Function to communicate with ChatGPT-4
def chat_with_gpt4(prompt):
    # Replace 'your_api_key_here' with your OpenAI API key
    openai.api_key = 'your_api_key_here'
    
    # Making a request to ChatGPT-4
    response = openai.Completion.create(engine='gpt-4', prompt=prompt, max_tokens=100)
    
    # Returning the response from ChatGPT-4
    return response.choices[0].text.strip()

# Creating the Gradio Interface
def chat_interface(prompt):
    response = chat_with_gpt4(f"Medical Assistant: {prompt}")
    return f"Medical Assistant: {response}"

iface = gr.Interface(fn=chat_interface, inputs="text", outputs="text")
iface.launch()

```
This script creates a simple chat interface where you can communicate with the ChatGPT-4 and get responses based on medical queries.

## Running the Chatbot <a name="running-the-chatbot"></a>

After creating the script, run it using Python:

```sh
python medical_chatbot.py
```

This will launch a local web server and you can interact with the chatbot through the browser.

## Conclusion <a name="conclusion"></a>
Congratulations! You have built a Medical Assistant Chatbot using ChatGPT and Python. The chatbot features an intuitive web interface, thanks to Gradio. As a final note, ensure that you keep your API key secure and avoid exposing it in public repositories.


## References <a name="references"></a>
- [ChatGPT API Documentation](https://platform.openai.com/docs/api-reference/completions/create)
- [Gradio Documentation](https://gradio.app/docs/)
- [ChatGPT in Python for Beginners - Build A Chatbot](https://www.youtube.com/watch?v=pGOyw_M1mNE&t=216s)
