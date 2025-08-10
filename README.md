This repositery explores the effectiveness of two approaches for inducing word tags.
The first approach involves the use of a Hidden Markov Model (HMM) trained with an unsupervised algorithm to generate word tags.
The second approach applies the K-means clustering algorithm on Bidirectional Encoder Representations from Transformers (BERT) embeddings to achieve the same objective.
The performance of these two models is evaluated using different measures.

Setup:

To run this code you can simply make a copy of the uploaded notebook on collab and run the code there.

Here is a collab link for the notebook

https://colab.research.google.com/drive/15mA-qSjVeRz406O6z0blec-betWLsM-9?usp=sharing


Notes: 

I used Google Drive to load and save the dataset and intermediate results (like embeddings).
For the code to work, either the same folders must be replicated in one's google drive, or the pathes should be adjusted properly to account for this.

Also, when you reach the part with getting the embeddings using BERT, it is better to switch the run time to a GPU.
The code was written to utilize the GPU capabilities and it will run much faster on a GPU. (4 hours on a modren CPU vs 5 min on a T4 GPU)

Also, note that the Unsupervised training for the HMMs will take a significant amount of time (around 10 hours combined).
