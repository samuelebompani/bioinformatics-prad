1. The considered problem
2. The machine learning approaches applied to solve it
3. The experimental set-up
4. The results obtained

1. THE PROBLEM

Prostate cancer is the second most common cancer in men worldwide. Its incidence is influenced by age, family history, genetic factors, and race. Localized prostate cancer can vary in behavior, ranging from aggressive to indolent forms. Risk stratification systems have been developed to predict progression and guide treatment decisions based on clinical and pathological factors. Molecular features play a crucial role in improving risk stratification and treatment approaches.

An omic is a suffix used to refer to different fields of study that involve comprehensive analysis of a specific biological component or aspect. It typically denotes a multidimensional approach to studying biological systems on a large scale, encompassing various molecular components, such as genes (genomics), proteins (proteomics), metabolites (metabolomics), and more. The omic sciences aim to understand the complex interactions and functions of these components to gain insights into biological processes.

There are three main approaches to multi-omics clustering: early, middle and late integration. Early integration combines all omic data into one matrix and applies single-omic clustering, but it overlooks the different distributions of values across omics. Middle integration builds a single model that considers all omics, incorporating joint dimension reduction and similarity-based analyses. Feature selection is essential due to the high dimensionality and complexity of the data, but similarity-based methods offer improved runtime and reduced reliance on feature selection. Late integration clusters each omic separately and then integrates the results, ignoring consistent interactions across omics.

Our goal is to discover disease subtypes in the prostate adenocarcinoma TCGA dataset and compare the results with the work done by the The Cancer Genome Atlas Research Network, which used an integrative clustering model on multi-omics data. The omic we are going to consider are mRNA, miRNA and protein expression data. The approach we are going to use involves using the PAM algorithms on various matrices obtained by integrating the omic data.  

The PAM (Partitioning Around Medoids) algorithm is a clustering algorithm used to group data points into clusters based on their similarity. It is an extension of the k-medoid algorithm and is often employed in data mining and machine learning applications. Unlike k-means, which uses means as cluster representatives, PAM employs medoids, which are actual data points within the cluster. Medoids are less sensitive to outliers and can provide better cluster representations when dealing with non-linear or asymmetric data. In summary, the PAM algorithm iteratively optimizes the selection of medoids to minimize the dissimilarity between data points within a cluster, aiming to create meaningful and cohesive clusters in the data set.

iCluster cos'è

2. THE MACHINE IS LEARNING (?!)

early integration
middle integration: snf, mean, nemo

pam
spectral clustering

NEMO
Traditional approaches to multi-omics analysis have limitations. NEMO constructs inter-patient similarity matrices for each omic, integrates them into one network, and performs clustering based on the integrated network. This approach is computationally efficient and does not require iterative optimization.

3. CHE EXPERIMENTI

confronto con iCluster con rand, adjustedrand, nmi
grafico? 

4. RISULTATI 

???????

Despite progress, there is still much to uncover about the molecular basis of prostate cancer and its implications for risk stratification. Further research, using integrative multi-omics analysis and exploring novel clustering methods, such as NEMO, can enhance our understanding of prostate cancer and lead to more effective risk assessment and treatment strategies.
