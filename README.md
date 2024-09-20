
# 🏷️ NOTE:
- The modified answer notebooks (`KarateClub_GCN_introduction.ipynb` and, `NetworkX_tutorial.ipynb`) are available in the repository.
- The answer sheet, including screenshots form Task 2 is in the `IT21170966_labsheet6_Answer.docx` word document.
  
# Deep Learning – Lab 6 - Graph Neural Networks

## 🚀 Tasks 

1.	Upload the NetworkX jupyter notebook file (i.e.,NetworkX_tutorial.ipynb) to google colab root directory.  
    - Run the above code and understand it.
    - Complete the code sections to get the degree matrix and Laplacian matrix of the created random graph.
    - Calculate the graph density of the random graph in the code. Use the below equation (D = graph density, |V| = number of nodes and |E| = number of edges).
    - Increase the N value from 20 (original value) to 200 with multiple N values in between and observe the change of graph density and degree distribution (i.e., histogram plot). Explain what you observe and write the answer in a word file.   
    <p align="center">
      <img src="https://github.com/user-attachments/assets/31dd07b8-aba2-49db-881a-23155f41f5c7" alt="Sublime's custom image"/>
    </p>


2.	In the KarateClub dataset based GCN code,  we use semi-supervised training approach along with the transductive leaning method.
    - Explain the differences between supervised learning, self-supervised learning and semi-supervised learning methods
    - Explain the differences between transductive learning and inductive learning.

3.	Upload the KarateClub dataset based GCN jupyter notebook file (i.e., KarateClub_GCN_introduction.ipynb ) to google colab root directory.
    - In this code, we use Zachary’s karate club network dataset.
    - Run the above code and understand it.
    - Increase the number of epochs from 50 to 500 and observe the change in validation accuracy and write what you observe in the word file.
    - Experiment without self-loops added to GCNConv() layers in the GCN() model and detail the model accuracy increase/decrease in the word file. 
    - Increase the number of GCNConv() layers in the GCN() model upto 8 layers from original 3 layers. Detail the accuracy increase/decrease in the word file.
        - In_channels and out_channels in GCNConv() can be considered as hyper-parameters and you can use the best performing values you find.
        - Add skip connections between some of the GCNConv() layers and try to see if that can improve the model performance.
        - Detail what you observe in the word file.
          
4.	Explain the differences between Message Passing GNN, graph convolution network (GCN), graph attention network (GAT) and GraphSAGE.  Write the answers in the word file.



___________     
<sub><sup>📌 *documented by @IndudiniThennakoon 2024* </sup></sub>
