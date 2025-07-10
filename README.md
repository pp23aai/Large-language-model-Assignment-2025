BERT2BERT Summarization Project


Overview

I’m excited to present the BERT2BERT Summarization Project. In this work, I fine-tuned a BERT2BERT model an encoder-decoder framework built on the BERT architecture to create concise, rephrased summaries using the CNN/DailyMail dataset. My goal was to assess its effectiveness for abstractive summarization, especially under resource-limited conditions, and I found the process both challenging and rewarding.
Project Contents

I adapted BERT, which I initially knew for its text understanding capabilities, into a summarization tool by using two BERT models: one to encode the input text and another to decode the summary. I relied on the Hugging Face transformers and datasets libraries to implement and test my approach. In my report, I’ve detailed the training process, evaluated performance using metrics like ROUGE and BLEU, and analyzed the summaries I generated.
Getting Started

Environment Setup: I installed Python and the necessary libraries using pip:
pip install transformers datasets torch


Dataset Acquisition: I obtained the CNN/DailyMail dataset from Hugging Face. Due to my hardware constraints, I worked with a subset (10,000 training, 1,000 validation, 1,000 test examples).

Execution: I ran the model on a GPU with 8GB memory, using a batch size of 2 and a learning rate of 2e-5. I recommend adjusting these settings based on your setup.
Review Results: I tracked progress over 7,000 steps and documented the metric trends and summary examples in my report.

Key Information

Training Process: I conducted training over three epochs, using mixed precision (FP16) to save memory, and applied the AdamW optimizer with a warm-up phase, which I found effective.
Performance: I was pleased to see steady improvement, with my model achieving a ROUGE-1 score of 17.91 and a BLEU score of 1.99. The summaries were mostly coherent, though I noticed they sometimes missed key details.
Limitations: I realized this approach works best with small datasets and modest hardware. I think larger datasets or advanced techniques could enhance the results.

 
