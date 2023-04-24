# 💫 StarCoder

## What is this about?
StarCoder💫 is a language model trained on source code and natural language text. Its training data incorporates more that 80 different programming languages as well as text extracted from github issues and commits and from notebooks.

## Fine-Tuning
As a decoder model, StarCoder can be fine-tuned to achieve multiple downstream tasks. Our interest in this part is to fine-tune StarCoder in order to make it follow instructions. [Instruction fine-tuning](https://arxiv.org/pdf/2109.01652.pdf) has gained a lot of attention recently as it proposed a simple framework that teach language models to align with human needs. That procedure requires the availability of instruction datasets, which contain instruction - answer pairs. Unfortunately such datasets are not ubiquitous but thanks to Hugging Face 🤗's [datasets](https://github.com/huggingface/datasets) library we can have access to some useful proxies.

### Code Alpaca 
[Code Alpaca](https://huggingface.co/datasets/HuggingFaceH4/CodeAlpaca_20K) is a dataset of about 20K prompt - completion pairs generated by the techniques in the [Self-instruct](https://arxiv.org/abs/2212.10560) paper applied to text-davinci-003. 
