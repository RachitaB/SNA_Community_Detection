# SNA_Community_Detection

This repository contains an implementation of community detection algorithms, namely the Clique Percolation Method (CPM) and Girvan-Newman algorithm, applied on the polbooks.gml dataset. The goal is to identify communities within the social network represented by the dataset.

## Dataset

The dolphins.gml dataset is included in the repository. It represents an undirected social network of frequent associations between 62 dolphins in a community living off Doubtful Sound, New Zealand.

## Algorithms

### Clique Percolation Method (CPM)

The Clique Percolation Method is a community detection algorithm based on finding overlapping cliques in a network. It works by first identifying all k-cliques in the graph and then merging the cliques that overlap in k-1 nodes. The resulting overlapping k-cliques form communities within the network.

### Girvan-Newman Algorithm

The Girvan-Newman algorithm is a hierarchical divisive algorithm that detects communities by iteratively removing edges with high betweenness centrality. It starts with the original network and calculates the betweenness centrality of all edges. The edge with the highest betweenness centrality is removed, and the process is repeated until no edges remain. The resulting disconnected components form the communities.
