# PEFT
## Overview
- Fine-tuning large language models (LLMs) is resource-intensive, requiring significant computational power and time.
- Parameter Efficient Fine-Tuning (PEFT) methods have been devised to tackle these challenges by updating only a fraction of the model parameters.
- PEFT encompasses techniques like LoRA and Prompt Tuning, which streamline the adaptation of LLMs for targeted tasks.

![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*4LOEgon8uwQrwAPU_pzY4w.png)

- This novel approach offers several advantages, making it a compelling strategy for efficient model adaptation.

## Advantages of PEFT
- `Efficient Memory Utilization:` PEFT reduces memory requirements by updating only a subset of model parameters. This is crucial for large LLMs with millions to billions of parameters, enabling fine-tuning even on hardware with limited memory, like a single GPU, and avoiding the need for expensive distributed GPU clusters.

- `Minimized Catastrophic Forgetting:` PEFT prevents catastrophic forgetting by freezing most model weights and updating specific parameters. This preserves previously learned knowledge, ensuring that fine-tuning for a new task doesn't harm performance on earlier tasks, allowing efficient adaptation to multiple tasks.

- `Flexibility and Versatility:` PEFT offers various methods with trade-offs in parameter and memory efficiency, training speed, model quality, and inference costs. This flexibility allows developers to choose the most suitable method for their needs, tailoring fine-tuning to strike the right balance between performance and resource requirements.

- `Lower Computational Costs:` PEFT reduces computational costs by updating fewer parameters, making it cost-effective for organizations and researchers with limited budgets or hardware resources. It maximizes compute efficiency and accelerates development processes.

## Techniques
1. Lora - Qlora
2. Prefix Tuning
3. P-Tuning
4. Prompt Tuning
5. AdaLoRA
6. Multi-task prompt tuning, etc

Happy Coding!!