# Unsupervised Inductive Node Representation Learning For Dynamic Graphs
#W. -G. Zhou and K. Abbas, "Unsupervised Inductive node representation learning for dynamic graphs," in IEEE Access, doi: 10.1109/ACCESS.2025.3553377.
keywords: {Representation learning;Graph neural networks;Training;Contrastive learning;Biological system modeling;Adaptation models;Social networking (online);Proteins;Evolution (biology);Data models;Dynamic Graph;Graph Representation Learning;Graph Neural Network;Unsupervised Graph Neural Network},

Graphs are used to model many real-world systems, like social networks (friendships), communication networks (email exchanges), and biological networks (interactions between proteins). To understand these systems, we often convert graphs into simpler mathematical representations called **embeddings**, which help analyze patterns and relationships between nodes (people, proteins, etc.).  

Most existing methods work on **static graphs**, meaning they don’t consider how connections change over time. However, in reality, relationships evolve—people make new friends, emails are sent at different times, and proteins interact dynamically. Some existing **dynamic graph models** exist, but they either need labeled data (which is not always available) or struggle to handle large networks.  

To solve this, we developed an **Unsupervised Dynamic Graph Neural Network (UDGNN)** that learns **without labeled data** and efficiently processes large, evolving graphs. Our approach:  
1. **Learns from graph changes over time** without needing predefined labels.  
2. **Uses a smart edge sampling strategy** to handle large networks efficiently.  
3. **Creates embeddings that remain stable over time**.  

We tested our model on five real-world datasets (social, communication, and biological networks) and compared it with **10 existing methods**. Our model performed better at capturing changes in graphs while using less memory, making it practical for real-world applications like **detecting unusual behavior in social networks or predicting protein functions in biology**.

Please extract the files keep *unsupervisedInductiveNodeRepresentationGenrationForDynamicGraphs* and *data* direcorty under same parent directory, and run the main_*.py. To use your own data see the src/loader/dataset_loader.py and make changes accordingly.
To change the sampling strategy.. change: models.DGNN._initialize_embeddings_HebbianImplementedDGNN.edge_sampling_strategy='deepwalk' #deepwalk,node2vec, None
**Keywords**: Unsupervise learning on graphs, DynamicNodeEmbedding, GraphRepresentationLearning, Unsupervised graph representation learning, Inductive representation generation. 
 

**Requirements**
pip install 
pthon>=3.6 
pip install networkx==2.3 tensorflow==1.14.0  numpy==1.19.5 tqdm==4.40.0 pandas==1.3.2 Keras==2.3.1 matplotlib==3.5.2 torch==1.9.0 node2vec==0.4.3 sklearn==0.0 qc-procrustes  scipy==1.7.3 pickle5 gensim==4.2.0

----
