# Detection_of_Illegal_Bitcoin_Transactions_and_Anti-Money_Laundering
In response to the challenges such as the strong concealment of illegal nodes and the extremely unbalanced sample distribution in the Bitcoin transaction network, a detection framework integrating graph neural networks and ensemble learning was proposed. The experiment was based on the Elliptic dataset, and the performance differences of four graph representation learning models (GCN, GAT, GraphSAGE, and GIN) in the identification of illegal nodes were compared and analyzed. Furthermore, a hybrid model coupling GIN with XGBoost was proposed.

Project Name: Research on Illegal Bitcoin Transactions Detection and Anti-Money Laundering Based on Graph Neural Networks
Research Question: In response to the challenges such as the strong concealment of illegal nodes and the extremely imbalanced sample distribution in the Bitcoin transaction network, a detection framework integrating graph neural networks and ensemble learning has been proposed. 

Dataset Description: Public Elliptic dataset
elliptic_txs_classes  Transaction address category, totaling 203,769 addresses, including illegal addresses (1), legal addresses (0), and unknown addresses
elliptic_txs_edgelist  Transaction address fund flow, totaling 234,355 fund flows
elliptic_txs_features  Transaction address features, each transaction address includes 166-dimensional features. The first 94 features represent local information about the transaction, including time step, input/output quantity, transaction fee, output quantity, and aggregated numbers, such as the average BTC received/spent by input/output (expenditure) and the average incoming quantity related to input/output transactions. The remaining 72 features are aggregated features, obtained by using transaction information to obtain the same information data (input/output quantity, transaction fee, etc.) from the central node backward/forward one hop (input/output quantity, transaction fee, etc.). 

Experimental code: experience.ipynb
Installation of libraries: os, random, numpy, pandas, scipy
torch (PyTorch v2.7.1 + cu118), torch_geometric (PyG v2.7.0)
xgboost (XGBClassifier), scikit-learn (v1.8.0, including preprocessing, metrics, manifold, etc. modules) networkx, python-louvain (community_louvain)
matplotlib, seaborn

The document includes all the codes and result graphs related to the course report.
