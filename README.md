# Large-language-model-Assignment-2025
BERT2BERT Summarization Project

Overview
Welcome to the BERT2BERT Summarization Project. This initiative involves fine-tuning a BERT2BERT model—an encoder-decoder framework based on the BERT architecture to generate concise, rephrased summaries using the CNN/DailyMail dataset. The project aims to evaluate its effectiveness for abstractive summarization, particularly in resource-constrained environments.
Project Contents

The project adapts BERT, originally designed for text understanding, into a summarization tool using two BERT models: one for encoding input text and another for decoding summaries.
It utilizes the Hugging Face transformers and datasets libraries for implementation and testing.
The report includes details on the training process, performance metrics (e.g., ROUGE, BLEU), and an analysis of the generated summaries.

Getting Started

Environment Setup: Install Python and the required libraries via pip:
pip install transformers datasets torch


Dataset Acquisition: Obtain the CNN/DailyMail dataset from Hugging Face. Due to hardware limitations, we used a subset (10,000 training, 1,000 validation, 1,000 test examples).
Execution: Run the model on a GPU with 8GB memory. We used a batch size of 2 and a learning rate of 2e-5; adjust as necessary for your setup.
Review Results: Refer to the report for metric trends and summary examples, tracked over 7,000 training steps.

Key Information

Training Process: Conducted over three epochs with mixed precision (FP16) to optimize memory usage, employing the AdamW optimizer with a warm-up phase.
Performance: The model improved steadily, achieving a ROUGE-1 score of 17.91 and a BLEU score of 1.99. Summaries were generally coherent but occasionally omitted key details.
Limitations: Best suited for small datasets and modest hardware. Enhancements could involve larger datasets or advanced techniques.

 
