### Extending experiments of UAT on MASSIVE dataset

- (1) creating a target classification model:
    - creating a multi-lingual BERT classifier for domain classification - MASSIVE has 18 domains. 
    - Using `bert-base-multilingual-cased` trained on validation dataset of MASSIVE (~ 100k utterances) for 3 epochs and achieve 85% accuracy on test dataset.
    - Result & code is shown in `Finetune domain classifier model.ipynb` notebook.


- (2) adversarial data filtering from MASSIVE training set (using training set as unlabeled data)
    - Using [sentence transformers/paraphrase-multilingual-miniLM](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2) to get sentence embeddings
    - running FAISS search and/or cosine similarities on the embeddings




