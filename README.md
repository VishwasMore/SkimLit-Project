# SkimLit-Project
The purpose of this notebook is to build an NLP model to make reading medical abstracts easier

## Data 

Since we'll be replicating the paper above (PubMed 200k RCT), let's download the dataset they used. We can do so from the authors GitHub: https://github.com/Franck-Dernoncourt/pubmed-rct

## Modelling

We will be building 6 Models 

* Model 0: Baseline Model (TF-IDF Multinomial Naive)
* Model 1: Conv1D with token embedding
* Model 2: Tensorflow Hub Feature Extractor
* Model 3: Conv1D with character embeddings
* Model 4: Combining prerained token embedding + character embedding (hybrid embedding layer)
* Model 5: Transfer learning with pretrained token embeddings + character embeddings + positional embeddings
