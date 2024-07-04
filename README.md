# ChatGPT-Prompt-Enigineering
Welcome to the repository of codes from the ChatGPT Prompt Engineering course by Deeplearning.AI. This repository includes various implementations of prompt engineering techniques such as expanding, guidelines, transforming, summarizing, inferring, iterative processing, and chatbot development.


# Overview
This repository showcases practical applications of prompt engineering strategies for ChatGPT, including:

* Expanding: Techniques for elaborating on initial prompts to generate more detailed outputs.
  
* Guidelines: Implementing specific instructions or constraints to guide the generation process.
  
* Transforming: Methods for changing the style or format of the generated text.
  
* Summarizing: Approaches to condense large amounts of information into concise summaries.
  
* Inferring: Using prompts to infer or extract specific information from text.
  
* Iterative Processing: Iterating over prompts and responses to refine outputs.
  
* Chatbot: Building a conversational agent using various prompt engineering strategies.


# Code Description
* expand_prompt.ipynb: Demonstrates techniques for expanding prompts to generate more comprehensive responses.
  
* guidelines.ipynb: Shows how to incorporate guidelines and constraints into prompts to influence the output.
  
* transforming.ipynb: Provides methods for transforming the output style or format.
  
* summarizing.ipynb: Contains examples of summarization techniques to condense information.
  
* inferring.ipynb: Illustrates how to infer specific details from a given prompt.
  
* iterative.ipynb: Shows how to refine responses through iterative prompt processing.
  
* chatbot.ipynb: Implements a simple chatbot using the aforementioned prompt engineering techniques.


# Code Example
Here is an example of how to use the OpenAI API for generating completions with a prompt:

```
import openai
import os

def get_completion(prompt, model="gpt-3.5-turbo", temperature=0): 
    messages = [{"role": "user", "content": prompt}]
    response = openai.ChatCompletion.create(
        model=model,
        messages=messages,
        temperature=temperature, 
    )
    return response.choices[0].message["content"]
```
In this code:

* get_completion is a function that sends a prompt to the OpenAI API and retrieves the model's response.
  
* You can adjust the model parameter to specify different versions of GPT.
  
* The temperature parameter controls the randomness of the response.
