# Fine-tuning Llama2-Chat Model with QLoRA on OpenOrca dataset

This repository contains the code and data used to fine-tune the Llama2-Chat model using the 4-bit quantisation QLoRA (Quantization with Low Rank Approximation) PEFT technique on the OpenOrca dataset.

## Dataset Preprocessing
### OpenOrca-Clean
The [OpenOrca-Clean](https://huggingface.co/datasets/baaghi124/OpenOrca-Clean) dataset is a refined version derived from the original [OpenOrca](https://huggingface.co/datasets/Open-Orca/OpenOrca) dataset. 

### Llama2-OpenOrca-Clean
The [Llama2-OpenOrca-Clean](https://huggingface.co/datasets/baaghi124/Llama2-OpenOrca-Clean) dataset is tailored specifically for fine-tuning the Llama2-Chat model. It is derived from the [OpenOrca-Clean](https://huggingface.co/datasets/baaghi124/OpenOrca-Clean) dataset, further adapted to fit the llama prompt template. The dataset comprises a single column labeled "text," structured in the given format-

<img width="337" alt="Screenshot 2024-04-06 115410" src="https://github.com/aayushxrj/Llama-2-7B-Chat-OpenOrca/assets/111623667/b9f35f1d-5bcf-4d26-9e34-efbd4df7f744">


## Model Fine-tuning
### Model Details
- **Base Model:** [Llama-2-7B-Chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf)
- **Fine-tuning Technique:** 4-bit quantization using [QLoRA](https://arxiv.org/pdf/2305.14314.pdf) [PEFT](https://arxiv.org/pdf/2312.12148.pdf)
- **Dataset Used:** [Llama2-OpenOrca-Clean](https://huggingface.co/datasets/baaghi124/Llama2-OpenOrca-Clean)

The fine-tuning process involves training the Llama2-Chat model with 4-bit quantization using the QLoRA technique. This technique allows for efficient representation of model parameters while minimizing computational overhead.

## Official Models
**Llama-2-7B-Chat-OpenOrca**

Our [latest model](https://huggingface.co/baaghi124/Llama-2-7B-Chat-OpenOrca), fine-tuned with 1000 examples using 4-bit quantization QLoRA from Llama2-OpenOrca-Clean dataset, is now available.

