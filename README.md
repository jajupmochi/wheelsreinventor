# pygorithm
My realm of algorithms in Python.


| Models          | Papers | Surveys & Books | Math by hands      | Blogs & Videos                                                                                                                                                                                             | Demo codes         | Raw codes                                                                                                                     | My implementations | Why invent this? | Where it is used?                                                                                 | Pros & Cons                                                         | V.S. others | More... |
| --------------- | ------ | --------------- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | ----------------------------------------------------------------------------------------------------------------------------- | ------------------ | ---------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------- | ------- |
| MPNN     | :heavy_check_mark:<br> - [Neural message passing from quantum chemistry](https://proceedings.mlr.press/v70/gilmer17a.html)       |                 |                    |                                                                                                  | :heavy_check_mark: <br> - [Message-passing neural network (MPNN) for molecular property prediction](https://keras.io/examples/graph/mpnn-molecular-graphs/) | :heavy_check_mark: <br> - [Original code](https://github.com/brain-research/mpnn) <br> - [DGL NNConv in PyTorch](https://docs.dgl.ai/generated/dgl.nn.pytorch.conv.NNConv.html?highlight=nnconv), [DGL-LifeSci MPNNGNN using it](https://lifesci.dgl.ai/_modules/dgllife/model/gnn/mpnn.html), and [DGL-LifeSci MPNNPredictor](https://github.com/awslabs/dgl-lifesci/blob/master/python/dgllife/model/model_zoo/mpnn_predictor.py#L18) <br> - [Keras: Message-passing neural network (MPNN) for molecular property prediction](https://keras.io/examples/graph/mpnn-molecular-graphs/) |      |                                                                                                                   | - Molecule property prediction            |                  | 
| GCN     | :heavy_check_mark:<br> - [Semi-supervised classification with graph convolutional networks](https://arxiv.org/abs/1609.02907)       |                 |                    |  - [Keras: Node Classification with Graph Neural Networks](https://keras.io/examples/graph/gnn_citations)                                                                                           | - [Keras: Node Classification with Graph Neural Networks](https://keras.io/examples/graph/gnn_citations)   | - :heavy_check_mark:[DGL implementation (in Tensorflow)](https://docs.dgl.ai/en/0.6.x/_modules/dgl/nn/tensorflow/conv/graphconv.html#GraphConv) <br> - [DGL implementation (in PyTorch)](https://docs.dgl.ai/en/0.6.x/_modules/dgl/nn/pytorch/conv/graphconv.html#GraphConv) <br> - [Keras: Node Classification with Graph Neural Networks](https://keras.io/examples/graph/gnn_citations)  |                                                                                            |                       | - Molecule property prediction            |                  | |         
| GAT     | :heavy_check_mark:<br> - [Graph attention networks](https://arxiv.org/abs/1710.10903)       |                 |                    |     - :heavy_check_mark:[Graph Attention Networks (by the authors)](https://petar-v.com/GAT/) <br> - :heavy_check_mark:[Understanding Graph Attention Networks (GAT)](https://dsgiitr.com/blogs/gat/) <br> - [DGL: Understand Graph Attention Network](https://docs.dgl.ai/tutorials/models/1_gnn/9_gat.html) <br> - [Keras: Graph attention network (GAT) for node classification](https://keras.io/examples/graph/gat_node_classification/)                                                                                           | - :heavy_check_mark:[Understanding Graph Attention Networks (GAT) (in PyTorch)](https://dsgiitr.com/blogs/gat/) <br> - [DGL: Understand Graph Attention Network (in PyTorch)](https://docs.dgl.ai/tutorials/models/1_gnn/9_gat.html) <br> - [Keras: Graph attention network (GAT) for node classification](https://keras.io/examples/graph/gat_node_classification/)   | - [Original code](https://github.com/PetarV-/GAT) <br> - :heavy_check_mark:[DGL implementation (in Tensorflow)](https://docs.dgl.ai/en/0.6.x/_modules/dgl/nn/tensorflow/conv/gatconv.html#GATConv) <br> - [DGL implementation (in PyTorch)](https://docs.dgl.ai/en/0.6.x/_modules/dgl/nn/pytorch/conv/gatconv.html#GATConv) <br> - [DGL example for graph classification (in Tensorflow)](https://github.com/dmlc/dgl/blob/master/examples/tensorflow/gat/gat.py) <br> - [Keras: Graph attention network (GAT) for node classification](https://keras.io/examples/graph/gat_node_classification/)    |                                                                                            |                       | - Molecule property prediction            |                  | |         
| GRU             |        |                 | :heavy_check_mark: | :heavy_check_mark:<br> - [Understanding GRU Networks](https://towardsdatascience.com/understanding-gru-networks-2ef37df6c9be)                                                                              | :heavy_check_mark: <br> - [Message-passing neural network (MPNN) for molecular property prediction](https://keras.io/examples/graph/mpnn-molecular-graphs/) | :heavy_check_mark: <br> - [Keras GRUCell](https://github.com/keras-team/keras/blob/v2.8.0/keras/layers/recurrent.py#L1718) |                    |                  | NLP: translation                                                                                  |                                                                     |             |         |
| Transformer     |        |                 |                    | :heavy_check_mark:<br> - [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/)                                                                                                 | :heavy_check_mark:<br> - [Keras MultiHeadAttention](https://github.com/keras-team/keras/blob/v2.8.0/keras/layers/multi_head_attention.py#L123-L516)                   |                                                                                                                               |                    |                  | - **GNN ([Aggregation function of MPNN](https://keras.io/examples/graph/mpnn-molecular-graphs/))** |                                                                     |             |         |
| RNN + Attention |        |                 |                    | :heavy_check_mark:<br> - [Attn: Illustrated Attention](https://towardsdatascience.com/attn-illustrated-attention-5ec4ad276ee3#ba24) <br> - [知乎：Attention in RNN](https://zhuanlan.zhihu.com/p/42724582) |                    |                                                                                                                               |                    |                  | NLP: translation                                                                                  | <span style="color:green">- Considering previous time steps</span> |             |         |