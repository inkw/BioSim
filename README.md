# BioSim
Measure similarity between random assays with accumulated PMID and GO terms using both node-based and content-based algorithm.
Spectral Clustering is based on similarity matrix.

////////////Data Processing////////////
#1 source data
https://www.ncbi.nlm.nih.gov/pubmed/
https://www.ebi.ac.uk/QuickGO/
Most of relationship terms, including is-a,part-of,regulate, are downloaded for further simlarity measure.

#2 connect path
A is a B ->B.A
A part of B-> B.A
regulates:combined relationship remained to be uncertain.
over ten thousand paths are connected. 

#3 sample

////////////Algorithm////////////
#1 node-based


#2 content-based


////////////Experiment////////////
Thousands of essays with specific GO terms are input to similarity algorithm metioned above to form similarity matrix.


////////////Clustering and Analysis////////////
#1 Spectral clustering
Spectral clustering is considered to be the best way for clustering as DBscan may result in data loss for noise point and K-means requires original data set.

#2 Frequency Calculatuon
Then, terms fequency is calculated with classified data set, which is to emphasis whether clustering results are correct.  
