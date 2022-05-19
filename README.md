# Repository for a project for CS224W Machine Learning with Graphs at Stanford


dataset: https://www.quandl.com/databases/SFA/data

model: https://github.com/srijankr/jodie/


As described in project report and poster, we constructed three graphs using SF3 dataset.

1. Directed Investor-Investor Graph: two investors share an edge if they invest in the same stock in subsequent quarters.  This graph is used for role detection (HITs analysis, PageRank analysis, and Motif analysis)

2. Undirected Investor-Investor Graph: two investors share an edge if they invest in the same stock in a same quarter.  This graph is used for community detection (Louvain algorithm)

3. Investor-Stock Bipartite Graph: an investor and a stock have an edge if an investor invests in a stock. This graph is directly fed into JODIE.  Edge features are crafted from SF1 dataset.


For evaluation, we calculate average quarterly returna and holding periods of each investor in Investor_Summary.ipynb, and compared those indicators with the results of role detection and community detection in Evaluation.ipynb. 
