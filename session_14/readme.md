# Python code generator using Transformer

## Dataset Preparation:
1. The dataset used is [python_dataset](https://github.com/trinanjan12/Trinanjan_END_NLP_Program/tree/main/session_14/dataset) and the script for preprocessing the data could be found here [python_dataset_cleaning](https://github.com/trinanjan12/Trinanjan_END_NLP_Program/tree/main/session_14/dataset_preprocessing)
2. The dataset is processed using pygments tokenizer library. https://pygments.org/
3. spaces are considered as indentation
4. 'code' is decoder input 'obj' is encoder input![dataset_example](images/python_dataset.png)


## Glove training:
1. The dataset used is [Raw Python Code Corpus](https://figshare.com/articles/dataset/Raw_Python_Code_Corpus/11777217) , I have randomly chosen 5000 files outof 68k python files to create a corpus.
2. The corpus is processed using pygments tokenizer.
3. The training notebook could be found here [Glove training](https://github.com/trinanjan12/Trinanjan_END_NLP_Program/blob/main/session_14/glove_embs_training.ipynb)
4. This glove embedding is used in the transformer decoder embedding.


## Transformer training:
1. The transformer uses pretrained glove embedding
2. loss function is default ce loss
3. The training and inference script could be found here [transformer_training](https://github.com/trinanjan12/Trinanjan_END_NLP_Program/blob/main/session_14/trainsformer_training.ipynb)

## Sample Output:
![test1](images/test1.png)
![test2](images/test1.png)
![test3](images/test1.png)

## Next steps:
1. Try training glove embedding on bigger python corpus maybe
2. Maybe try different loss function
