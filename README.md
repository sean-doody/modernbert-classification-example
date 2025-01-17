# ModernBERT Fine-Tune: IMDB Example

This notebook contains a recipe for fine-tuning [ModernBERT-base](https://huggingface.co/answerdotai/ModernBERT-base) for a binary classification task. The [IMDB reviews dataset](https://huggingface.co/datasets/stanfordnlp/imdb) is used as a toy example, but the code can adapted for other workflows.

## Running the Code

- The notebook can be run on free-tier [Google Colab](https://colab.research.google.com) runtimes.
- I used a batch size of 4 and an eval batch size of 2 on a free T4 GPU runtime.
- While ModernBERT supports up to 8192 tokens, I kept this example to 1024 tokens. 
  - I wanted to test the performance of the model using a moderately sized max length.