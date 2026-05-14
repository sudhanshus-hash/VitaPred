# VitaPred: Prediction of Vitamin Interacting Residues in Vitamin Binding Proteins Using Evolutionary Information

VitaPred is a computational tool developed for predicting vitamin-interacting residues in vitamin-binding proteins from amino acid sequences.

Vitamins act as important cofactors in many enzymatic reactions. Identification of vitamin-binding residues can help in understanding enzyme activity, vitamin-protein interactions, and drug target development. VitaPred uses evolutionary information and machine learning models to predict residues interacting with vitamins and vitamin subclasses.

Web Server: https://webs.iiitd.edu.in/raghava/vaxinpad/protein.php


## Citation

Panwar, B., Gupta, S., and Raghava, G. P. S. Prediction of vitamin interacting residues in a vitamin binding protein using evolutionary information. BMC Bioinformatics, 14, 44, 2013.
https://doi.org/10.1186/1471-2105-14-44

This tool and dataset is also available on Zenodo at 


## About the Research

Vitamins are essential cofactors involved in many metabolic and enzymatic reactions. Many vitamin-dependent enzymes are important drug targets, especially in diseases such as tuberculosis, malaria, cancer, and other metabolic disorders.

Experimental identification of vitamin-binding sites is difficult because many protein structures are unavailable and vitamin-protein interactions can be complex. Therefore, VitaPred was developed to predict vitamin-interacting residues directly from protein sequence information.

Data Compilation: Protein-vitamin interaction data were collected from SuperSite and Protein Data Bank structures. Ligand Protein Contact analysis was used to identify residues interacting with vitamins using a 5 Å distance cutoff.

Methodology: VitaPred uses machine learning models trained on binary sequence profiles and Position-Specific Scoring Matrix profiles. PSSM-based evolutionary information was found to improve prediction performance compared to binary sequence-based models.



## Key Features

### 1. Vitamin-Interacting Residue Prediction

Predictive Modeling: Allows users to submit protein sequences and predict vitamin-interacting residues.

VIR Prediction: Predicts general vitamin-interacting residues in vitamin-binding proteins.

Performance: The PSSM-based SVM model achieved MCC 0.53 for prediction of vitamin-interacting residues.



### 2. Vitamin Subclass-Specific Prediction

VitaPred provides separate prediction modules for different vitamin classes.

The tool predicts:

- Vitamin-interacting residues
- Vitamin A-interacting residues
- Vitamin B-interacting residues
- Pyridoxal-5-phosphate interacting residues

Vitamin A Prediction: The best PSSM-based model achieved MCC 0.48 for vitamin A-interacting residue prediction.

Vitamin B Prediction: The best PSSM-based model achieved MCC 0.61 for vitamin B-interacting residue prediction.

PLP Prediction: The best PSSM-based model achieved MCC 0.81 for pyridoxal-5-phosphate interacting residue prediction.



### 3. Evolutionary Information-Based Modeling

PSSM Profiles: VitaPred uses PSI-BLAST-generated Position-Specific Scoring Matrix profiles to capture evolutionary information.

Machine Learning Models: Several classifiers were tested, including Support Vector Machine, BayesNet, Naive Bayes, Complement Naive Bayes, Naive Bayes Multinomial, Random Forest, and IBk.

Best Classifier: SVM-based models using PSSM features performed best overall.

Independent Validation: The prediction modules were also evaluated on independent datasets for VIRs, VAIRs, VBIRs, and PLPIRs.

Standalone Software: VitaPred is also available as standalone software for large-scale sequence analysis.



## Applications

Vitamin-Binding Site Prediction: VitaPred can help identify vitamin-interacting residues in proteins when experimental structures are unavailable.

Drug Discovery: Since several vitamin-dependent enzymes are drug targets, VitaPred can support inhibitor design against vitamin-binding pockets.

Functional Annotation: The tool can help annotate vitamin-binding residues in newly sequenced proteins.

Enzyme Mechanism Studies: VitaPred can assist in studying enzyme activity and cofactor-binding mechanisms.

Protein-Ligand Interaction Research: The tool provides a computational framework for analyzing vitamin-protein interaction patterns.

PLP-Dependent Enzyme Analysis: VitaPred can help study pyridoxal-5-phosphate interacting residues in PLP-dependent enzymes.



## Contact and Authors

Prof. Gajendra P. S. Raghava  
Corresponding Author  

Email: raghava@iiitd.ac.in

Department of Computational Biology, Indraprastha Institute of Information Technology (IIIT Delhi), New Delhi, India.



## Support

This work was supported by the Council of Scientific and Industrial Research and the Department of Biotechnology, Government of India.
