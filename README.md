# Document Classification with BERT

This notebook presents a simple document classification procedure using a pre-trained BERT model.

Overview of the notebook:

* Loading BERT model & BERT tokenization - we use the `transformers` library from `huggingface` to load a 'bert-base-uncased' model with pre-trained weights. We then utilize appropriate tokenization functions from the same library
* Model definition and forward function - we create a PyTorch model with the BERT, Embedding and Linear layers, with CrossEntropy on top of that
* Training - again from `huggingface`, we'll use a Trainer instance to automate this process and enable simple reporting to `wandb.ai`
* Test Set Evaluation - we evaluate our model on the test set, using the same trainer instance from the previous section
* Report of results - at the end, we present a confusion matrix for predictions on the test set

[wandb training dashboard](https://wandb.ai/radswn/huggingface)
