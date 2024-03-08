# QLoRA - Quantized and Low-Rank Adaptation of LLM
## Overview
- In this method, the original pre-trained weights of the model are quantized to 4 bit and keep fixed during fine-tuning.
- Then, a small number of trainable parameters in the form of low-rank adapters are introduced during fine-tuning.
- These adapters are trained to adapt the pre-trained model to the specific task it is being fine tuned for, in 32 bit floating point format.
- When it comes to computations (like forward and backward passes during training , or inference), the 4bit quantized weights are de-quantized back to 32 bit floating point numbers.
- After the fine-tuning process, the model consists of the original weights in 4bit form, and the additional low rank adapters in their higher precision format.
- The additional low rank adapters in the QLoRA method are in a higher precision format, typically 32 bit floating point(bfloat), for a few reasons:
  - Higher precision allows the model to capture more subtle patterns in the data. This is particularly important for the low-rank adapters, as they are responsible for adapting the pre-trained model to the specific task it is being fine-tuned for.
  - Training neural networks involves a lot of incremental updates to the weights. Weights in a higher precision format ensures that updates are accurately captured.
  - GPUs are optimized for 32 bit operations.

Happy Coding!!