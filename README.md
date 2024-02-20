# UnsupervisedInductiveNodeRepresentationForDynamicGraphs
In this project we have given framework for unsupervised learning for dynamic graphs as well as generating node embedding inductively for other snapshots of the graphs.
**
Unsupervised learning for inductive node embedding generation for dynamic graphs
**. 

Please extract the files keep *unsupervisedInductiveNodeRepresentationGenrationForDynamicGraphs* and *data* direcorty under same parent directory, and run the main_*.py. To use your own data see the src/loader/dataset_loader.py and make changes accordingly.
To change the sampling strategy.. change: models.DGNN._initialize_embeddings_HebbianImplementedDGNN.edge_sampling_strategy='deepwalk' #deepwalk,node2vec, None
**Keywords**: Unsupervise learning on graphs, DynamicNodeEmbedding, GraphRepresentationLearning, Unsupervised graph representation learning, Inductive representation generation. 
 

**Requirements**
pip install 
pthon>=3.6 
pip install networkx==2.3 tensorflow==1.14.0  numpy==1.19.5 tqdm==4.40.0 pandas==1.3.2 Keras==2.3.1 matplotlib==3.5.2 torch==1.9.0 node2vec==0.4.3 sklearn==0.0 qc-procrustes  scipy==1.7.3 pickle5 gensim==4.2.0

----
