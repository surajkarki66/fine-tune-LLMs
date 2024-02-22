# fine-tune-LLMs
## Overview
Fine-tuning Large Language Models (LLMs) involves adapting pre-trained models to specific tasks or domains by further training them on task-specific data. This process is particularly popular in natural language processing (NLP) tasks where LLMs, such as GPT (Generative Pre-trained Transformer) models, have demonstrated remarkable performance across various domains.

## Fine Tuning Techniques
### 1. Adapter-based Learning
- Adapter-based learning is a method for efficiently adapting pre-trained language models (LMs) to new tasks or domains while minimizing computational resources and data requirements. Instead of fine-tuning the entire pre-trained model, adapter-based learning involves adding task-specific modules, called adapters, to the pre-trained model's architecture.
- For example: PEFT, Lora - Qlora

### 2. Full-model Fine-tuning
- Full model fine-tuning, also known as end-to-end fine-tuning, involves updating all parameters of a pre-trained language model (LM) during training on a specific downstream task. Unlike adapter-based learning, where only task-specific adapters are trained while keeping the pre-trained model parameters fixed, full model fine-tuning modifies all parameters of the original pre-trained model.


### 3. Prompt based Fine-tuning
- Prompt-based fine-tuning involves fine-tuning a pre-trained language model (LM) by providing task-specific prompts or instructions during the training process. Instead of training the model to directly predict the next word or token in a sequence, the model is trained to generate text conditioned on a given prompt, which guides its generation toward the desired task or domain.
- For example: One shot learning, Few shot learning


Happy Coding!!


