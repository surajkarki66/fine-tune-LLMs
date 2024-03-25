# Prompt-engineering

## Overview

- Prompt engineering refers to the process of designing and refining prompts to achieve specific outcomes in natural language processing (NLP) tasks, particularly in the context of training large language models like GPT (Generative Pre-trained Transformer).
- It involves crafting prompts that effectively guide the model to generate desired responses or perform desired tasks.

## Types

Three popular techniques for helping a Large Language Model solve a new task are zero-shot, one-shot, and few-shot prompting.

### 1. Zero-Shot Prompting

- It refers to simply asking the model to do something it was not trained to do.
- The word "zero" refers to giving the model no examples of how this new task should be solved.
- For example, suppose you ask a model to translate a sentence from one language to another.
- For example, "write a youtube script for my tech review channel"

### 2. One-Shot Prompting

- One piece of data or guideline given before completing request.
- Formula:  "Using this Example 1 as reference, then [prompt]."
- For example, "Write a youtube script for my tech review channel related to latest MacOS."

### 3. Few-Shot Prompting

- Asking a LLM to solve a new task while providing examples of how the task should be solved.
- Formula: "Using these Example 1, 2, 3 as reference, then [prompt]."
- Example:
  "Here are some examples of sentiment classification:
  Product A is awesome! //positive
  Product A is bad! //negative
  Product A doesn't work! //negative
  Product B is fantastic! //positive
  Product B is amazing! //positive
  Product B is bad! //negative

    Based on the examples, classify this:
    Product A is great!"

Happy Coding!!
