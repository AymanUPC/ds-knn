# DS-kNN
The OpenML clustering ground-truth for testing the DS-kNN algorithm. It includes a sample of 203 annotated datasets with their topic-wise groups as visualised in the *proximity graph* in the image below. It shows the datasets from the sample as the nodes with their labelled names and the similarity relationships between datasets as edges with their annotated similarity scores in the range of [0,1]. Datasets in the same cluster are shown in the same colour.

![OpenML Data Lake Proximity Graph](/OpenML_Data_Lake_Proximity_Graph.png?raw=true "Output DS-kNN proximity graph")

## DS-kNN Clustering of Datasets Using Proximity Mining (Keeping the Data Lake in Form) (OpenML implementation)
This page is dedicated for the DS-kNN Clustering of Datasets Using Proximity Mining project by the [DTIM Research Group](http://www.essi.upc.edu/dtim) of the ESSI department, UPC. We provide here the main benchmark datasets and sources for experimental evaluation of techniques for dataset clustering by topic-wise groups from [OpenML](https://www.openml.org) data.

## Description
* **DS-knn_203ds_OpenML_datasets.csv:** Stores the information about the 203 datasets we retrieved from OpenML and which we annotated with their general subject-areas and more specific entity topics by examining their textual description from OpenML. Each dataset has its annotated subject and entity in the *"Subject_Cluster"* and *"Entity_Cluster respectively"*. The rest of the columns contain the *content metadata we collect about the overall statistics* of the attributes of the dataset and data stored in them. Those are described in our paper.

* **DS-knn_203ds_OpenML_attributes.csv:** Stores the information about the attributes from the 203 datasets sample we retrieved from OpenML. This includes the attribute names and the attribute types.

To retrieve the original datasets from OpenML using the APIs provided by them and the dataset IDs from our CSV files, please refer to the [OpenML API guide](https://openml.github.io/OpenML/Java-guide/).

## Built With

* [Java OpenML API](https://openml.github.io/OpenML/Java-guide/)
* [Postgres DB](https://www.postgresql.org/)
* [WEKA Machine Learning Environment](http://www.cs.waikato.ac.nz/ml/weka/)
* [Apache Lucene](http://lucene.apache.org/)

## Acknowledgements
We are sincerely thankful to all the annotators who have validated and collaborated in creating the ground-truth datasets for the experiments. We thank the collaborators from the school of Pharmacy for helping us with the annotation of the datasets.



