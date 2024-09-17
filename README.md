# Enhancing downstream tasks in Knowledge Graphs Embeddings: A Complement Graph-based Approach Applied to Bilateral Trade

This work was presented at 27th International Conference on Knowledge-Based and Intelligent Information & Engineering Systems (KES 2023).


## Abstract 

Forecasting international trade flows is crucial for understanding global economic activity and serving as critical economic indicators used by economists and policymakers with significant implications for respective countries' economic policies. However, this is a challenging task due to the complexity of the relationships between entities involved in international trade. While several approaches have been proposed, knowledge graph-based models have emerged as promising solutions for predicting international trade flows.

In this paper, we introduce a synthetic triple-generation algorithm for enhancing downstream tasks in knowledge graph embeddings based on the graph complement. The algorithm identifies missing relationships between entities by exploiting the complement graph and generates high-quality synthetic triples that improve the accuracy of predictions. We validate the generated triples using several knowledge graphs embedding methods and computing metrics. To perform an initial result screening, an international trade scenario is explored, demonstrating the effectiveness of the proposed approach in enhancing the performance of knowledge graph-based models for predicting international trade flows.

## The CEPII gravity database

The CEPII gravity database is a dataset containing information on bilateral trade flows between countries worldwide. The dataset is based on the gravity model of international trade, which states that the trade volume between two countries is proportional to their economic size and inversely proportional to the distance between them. More than 220 countries and territories are represented in this database, with details on trade flows, GDP, population, and other pertinent variables available from 1948 to the present. The dataset is available on the  [CEPII website](http://www.cepii.fr/CEPII/en/bdd_modele/).

## Experimentation Scenario

The followig figure presents our experimental scenario. Initially, the input triples are trained and tested as shown in Figure to establish a baseline for a given model. The baseline approach is called KB. KB+Synth1 use the KB and synthetic as Validation Data and KB+Synth2, KB combined with synthetic triples in Train/Test/Valid sets.

<p align="center">
  <img src="https://github.com/d1egoprog/SyntheticTriples/blob/main/img/test-cases.png?raw=true" alt="Experimentation Scenario"/>
</p>


### Run the TensorFlow + Jupyter Notebook locally

If preferred, a docker-compose file type is also available. Run the command to launch the TensorFlow + Jupyter Notebook ready-to-use environment.

``` bash
git clone https://github.com/d1egoprog/SyntheticTriples.git
cd SyntheticTriples/
```

Run the command to launch the TensorFlow + Jupyter Notebook ready-to-use environment

```  bash
docker-compose -p sandbox up -d
```

## Citations 

If this work is with your interest you can read the presented [paper](hhttps://www.sciencedirect.com/journal/procedia-computer-science) (Not Published Yet) and if you use it in your research please don't forget to cite 👍 this work, the suggested citation in BibTex format is:

``` BibTex
@article{Rincon-Yanez2023c,
author = {Rincon-Yanez, Diego and Mouakher, Amira and Senatore, Sabrina},
doi = {10.1016/j.procs.2023.10.364},
issn = {18770509},
journal = {Procedia Computer Science},
pages = {3692--3700},
publisher = {Elsevier},
title = {{Enhancing downstream tasks in Knowledge Graphs Embeddings: A Complement Graph-based Approach Applied to Bilateral Trade}},
url = {https://linkinghub.elsevier.com/retrieve/pii/S1877050923015223},
volume = {225},
year = {2023}
}
```

## Contact

For questions, feedback, or support, please contact us by opening an [issue](https://github.com/d1egoprog/SyntheticTriples/issues/new/choose). And contributing is always welcome.
