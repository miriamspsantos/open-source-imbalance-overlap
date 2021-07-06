# Open Source Contributions in Learning <br> from  Imbalanced and Overlapped Data
Code availability is a crucial aspect for the reproducibility of results. Well-established methods in the field of Imbalanced Learning are commonly found in several open-source implementations. Some of the most popular are [KEEL Software Tool](http://keel.es) and [WEKA workbench](https://www.cs.waikato.ac.nz/ml/weka/), among other [R and Python packages](#packages). This repository further identifies existing resources (code and/or data) related to the joint-study of Class Imbalance, Class Overlap and Data Complexity. 

For a comprehensive analysis of the joint-effect of Class Imbalance and Overlap, please refer to:

> M. S. Santos, P. H. Abreu, N. Japkowicz, A. Fernández, C. Soares, S. Wilk, J. Santos, On the joint-effect of Class Imbalance and Overlap: A Critical Review, 2021.

Data Complexity Measures with application on Imbalanced and Overlapped domains, as well as Open Directions for future research are thoroughly discussed in:

> M. S. Santos, P. H. Abreu, N. Japkowicz, A. Fernández, J. Santos, A Unifying View of Class Imbalance and Overlap: Key Concepts, Panorama and Open Avenues for Research, 2021.

<br>

----
## Dataset Benchmarking and Data Generation
### **Benchmark Datasets:**
Well-known data repositories include:

- UCI Machine Learning Repository [[Datasets]](http://archive.ics.uci.edu/ml/datasets.php)
- Kaggle Repository [[Datasets]](https://www.kaggle.com/datasets)
- OpenML [[Datasets]](https://www.openml.org/search?type=data)
- KEEL Dataset Repository [[Datasets]](https://sci2s.ugr.es/keel/datasets.php)

Regarding specific data characteristics, KEEL is perhaps the most popular repository. It provides a collection of both standard datasets as well as datasets targeted to imbalance learning, noisy and borderline example detection, and singular problems (multi-instance and multi-label datasets) [[Imbalanced Datasets]](https://sci2s.ugr.es/keel/imbalanced.php)


### **Data Generation and Visualisation:**
- **Data Generation**: Within the scope of artificially generated data, we recommend the [data generator](https://github.com/sysmon37/datagenerator/tree/newsampling) used in [[Wojciechowski2017]](). A comprehensive description of the generator may be found in [this repository](). 

- **Instance Space Analysis**: Regarding the characterisation of datasets comprised in well-known repositories, exploring [MATILDA](https://matilda.unimelb.edu.au/matilda/our-methodology) (Melbourne Algorithm Test Instance Library with Data Analytics ) is an interesting direction. It allows the visualisation of the distribution and diversity of existing benchmark and real-world instances, and the generation of new synthetic test instances at specific locations of the instance space (e.g. real-world-like instances, or instances with controllable properties) [[Code]](https://github.com/andremun/InstanceSpace)[[Munoz2018]](#Munoz2018)

<br>

---
## Class Overlap-Based Approaches:
Class Overlap-Based Approaches aim to address class imbalance and overlap simultaneously [[Santos2021a]](#paper1). Despite they often derive from distribution-based approaches to some extent (frequently focused on undersampling or oversampling), their inner operations are more attentive to class overlap. For a comprehensive review on class overlap-based approaches please refer to [[Santos2021a]](#Santos2021a) and [[Vuttipittayamongkol2021]](#Vuttipittayamongkol2021). 

The following approaches include open-source implementations:

- **OBU**: Overlap-based Undersampling 
[[Code]](https://github.com/fonkafon/Overlap_based_Undersampling)[[Vuttipittayamongkol2018]](#Vuttipittayamongkol2018). 

- **BoostOBU**: Improved Overlap-based Undersampling
[[Code]](https://github.com/fonkafon/BoostedOBU)[[Vuttipittayamongkol2020a]](#Vuttipittayamongkol2020a). 

- **NB-Basic, NB-Tomek, NB-Comm, NB-Rec**: Neighbourhood-based Undersampling
 [[Code]](https://github.com/fonkafon/NB-undersampling)[[Vuttipittayamongkol2020b]](#Vuttipittayamongkol2020b). 

- **A-SUWO**: Adaptive semi-unsupervised weighted oversampling
 [[Code]](https://github.com/Nekooeimehr/MATLAB-Source-Code-Oversampling-Methods)[[Nekooeimehr2016]](#Nekooeimehr2016) 

 - **PAIO**: Position characteristic-Aware Interpolation Oversampling 
[[Code]](https://github.com/zhutuanfei/PAIO)[[Zhu2020]](#Zhu2020)

- **CCR**: Combined Cleaning and Resampling algorithm
[[Code]](https://github.com/michalkoziarski/CCR)[[Koziarski2017]](#Koziarski2017)

- **G-SMOTE**: Geometric SMOTE
[[Code]](https://github.com/georgedouzas/geometric-smote)[[Douzas2019]](#Douzas2019)

- **EFIS-MOEA**: Ensemble with Feature and Instance Selection with Multi-Objective Evolutionary Algorithm
[[Code]](https://github.com/aFdezHilario/EFIS-MOEA)[[Fernandez2017]](#Fernandez2017)


- **MOSNS and MOSS**: Minimising Overlapping Selection under No-Sampling and Minimising Overlapping Selection under SMOTE [[Code]](https://ars.els-cdn.com/content/image/1-s2.0-S0169743919306070-mmc1.zip
)[[Fu2020]](#Fu2020)

- **ImGrid**: Imbalanced Grid Clusterer [[Code]](https://github.com/langus0/imgrid)[[Lango2017]](#Lango2017)


<br>

---
## Data Complexity Measures
Data Complexity Measures (DCM) are commonly used to characterise the difficulty of classification tasks through the analysis of certain data characteristics. Existing open-source implementations of complexity measures include:

- **DCoL**: Data Complexity Library (C++) [[Code]](https://github.com/nmacia/dcol)[[Orriols-Puig2010]](#Orriols-Puig2010)

- **ECoL**: Extended Complexity Library (R) [[Code]](https://github.com/lpfgarcia/ECoL)[[Lorena2019]](#Lorena2019)

- **ImbCoL**: Data Complexity Measures for Imbalanced Classification (R): [[Code]](https://github.com/victorhb/ImbCoL)[[Barella2018]](#Barella2018)

- **SCoL**: Simulated Complexity Library (R) [[Code]](https://github.com/lpfgarcia/SCoL)[[Garcia2020]](#Garcia2020)

- **mfe**: Meta-Feature Extractor (R) [[Code]](https://github.com/rivolli/mfe)[[Alcobaca2020]](#Alcobaca2020)

- **pymfe**: Python Meta-Feature Extractor (Python) [[Code]](https://github.com/ealcobaca/pymfe)[[Alcobaca2020]](#Alcobaca2020)

- **Metalearn**: Library of Meta-Learning Tools (Python) [[Code]](https://github.com/byu-dml/metalearn)

- **PyHard**: Instance Hardness Python package (Python) [[Code]](https://pypi.org/project/pyhard/)[[Smith2014]](#Smith2014)

<br>

---
## <span id="packages">Imbalanced Data Learning Software</span>

- `unbalanced`: Racing for Unbalanced Methods Selection (R) [[Code]](https://cran.r-project.org/web/packages/unbalanced)

- `smotefamily`: A Collection of Oversampling Techniques for Class Imbalance Problem Based on SMOTE (R) [[Code]](https://cran.r-project.org/web/packages/smotefamily)

- `ROSE`: Random Over-Sampling Examples (R) [[Code]](https://cran.r-project.org/web/packages/ROSE)

- `imbalance`: Preprocessing Algorithms for Imbalanced Datasets (R) [[Code]](https://cran.r-project.org/web/packages/imbalance)

- `imbalanced-learn`: Resampling techniques for Imbalanced Data  (Python) [[Code]](https://pypi.org/project/imbalanced-learn/)

- `smote_variants`: SMOTE variantes for Imbalanced Learning (Python) [[Code]](https://github.com/analyticalmindsltd/smote_variants)[[Kovacs2019]](#Kovacs2019)

- `multi-imbalance`: Python library for Multi-Class Imbalanced Classification (Python) [[Code]](https://github.com/damian-horna/multi-imbalance)[[Grycza2020]](#Grycza2020)


- `Multi_Imbalance`: An open-source software for multi-class imbalance learning [[Code]](https://github.com/chongshengzhang/Multi_Imbalance)[[Zhang2019]](#Zhang2019)


- `cluster-over-sampling`: Clustering based Oversampling Algorithms(Python) [[Code]](https://github.com/georgedouzas/cluster-over-sampling)[[Douzas2017]](#Douzas2017)[[Douzas2018]](#Douzas2018)

- `undersampling`: A Scala library for undersampling in Imbalanced Classification (Scala) [[Code]](https://github.com/NestorRV/undersampling)

<br>

---
## References:
<span id="Santos2021a">`[Santos2021a]`</span>
M. S. Santos, P. H. Abreu, N. Japkowicz, A. Fernández, C. Soares, S. Wilk, J. Santos, On the joint-effect of Class Imbalance and Overlap: A Critical Review, 2021.


<span id="Santos2021b">`[Santos2021b]`</span>
M. S. Santos, P. H. Abreu, N. Japkowicz, A. Fernández, J. Santos, A Unifying View of Class Imbalance and Overlap Key Concepts, Panorama and Open Avenues for Research, 2021.


<span id="Vuttipittayamongkol2021">`[Vuttipittayamongkol2021]`</span>
P. Vuttipittayamongkol, E. Elyan, A. Petrovski, On the class overlap problem in imbalanced data classification, Knowledge-based systems, 2021. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0950705120307607)


<span id="Vuttipittayamongkol2018">`[Vuttipittayamongkol2018]`</span>
P. Vuttipittayamongkol, E. Elyan, A. Petrovski, C. Jayne, Overlap-based undersampling for improving imbalanced data classification, in: International Conference on Intelligent Data Engineering and Automated Learning, Springer, 2018, pp. 689–697. [[Link]](https://link.springer.com/chapter/10.1007/978-3-030-03493-1_72)


<span id="Vuttipittayamongkol2020a">`[Vuttipittayamongkol2020a]`</span>
P. Vuttipittayamongkol, E. Elyan, Improved overlap-based undersampling for imbalanced dataset classification with application to epilepsy and parkinson’s disease, International journal of neural systems, 30(8), 2020. [[Link]](https://www.worldscientific.com/doi/10.1142/S0129065720500434)


<span id="Vuttipittayamongkol2020b">`[Vuttipittayamongkol2020b]`</span>
P. Vuttipittayamongkol, E. Elyan, Neighbourhood-based undersampling approach for handling imbalanced and overlapped data, Information Sciences 509 (2020) 47–70. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0020025519308114)


<span id="Nekooeimehr2016">`[Nekooeimehr2016]`</span>
I. Nekooeimehr, S. K. Lai-Yuen, Adaptive semi-unsupervised weighted oversampling (A-SUWO) for imbalanced datasets, Expert Systems with Applications 46 (2016) 405–416. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0957417415007356)


<span id="Zhu2020">`[Zhu2020]`</span>
T. Zhu, Y. Lin, Y. Liu, Improving interpolation-based oversampling for imbalanced data learning, Knowledge-Based Systems 187 (2020). [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0950705119303016)

<span id="Koziarski2017">`[Koziarski2017]`</span>
M. Koziarski, M. Wozniak, CCR: A combined cleaning and resampling algorithm for imbalanced data classification, International Journal of Applied Mathematics and Computer Science 27 (4) (2017) 727–736. [[Link]](https://sciendo.com/de/article/10.1515/amcs-2017-0050)

<span id="Douzas2019">`[Douzas2019]`</span>
G. Douzas, F. Bacao, Geometric smote a geometrically enhanced drop-in replacement for smote, Information sciences 501 (2019) 118–135. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0020025519305353)


<span id="Fernandez2017">`[Fernandez2017]`</span>
A. Fernández, C. J. Carmona, M. Jose del Jesus, F. Herrera, A pareto-based ensemble with feature and instance selection for learning from multi-class imbalanced datasets, International Journal of neural systems, 27(6), 2017. [[Link]](https://www.worldscientific.com/doi/abs/10.1142/S0129065717500289)


<span id="Fu2020">`[Fu2020]`</span>
G.-H. Fu, Y.-J. Wu, M.-J. Zong, L.-Z. Yi, Feature selection and classification by minimizing overlap degree for class-imbalanced data in metabolomics, Chemometrics and Intelligent Laboratory Systems 196, 2020. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0169743919306070)


<span id="Lango2017">`[Lango2017]`</span>
M. Lango, D. Brzezinski, S. Firlik, J. Stefanowski, Discovering Minority Sub-clusters and Local Difficulty Factors from Imbalanced Data, International Conference on Discovery Science. Springer, Cham, 2017. [[Link]](https://link.springer.com/chapter/10.1007/978-3-319-67786-6_23)



<span id="Wojciechowski2017">`[Wojciechowski2017]`</span>
S. Wojciechowski, S. Wilk, Difficulty factors and preprocessing in imbalanced data sets: an experimental study on artificial data, Foundations of Computing and Decision Sciences 42 (2) (2017) 149–176. [[Link]](https://sciendo.com/article/10.1515/fcds-2017-0007)


<span id="Munoz2018">`[Munoz2018]`</span>
M. A. Muñoz, L. Villanova, D. Baatar, K. Smith-Miles, Instance spaces for machine learning classification, Machine Learning 107 (1) (2018) 109–147. [[Link]](https://link.springer.com/article/10.1007/s10994-017-5629-5)


<span id="Orriols-Puig2010">`[Orriols-Puig2010]`</span>
A. Orriols-Puig, N. Macia, T. K. Ho, Documentation for the data complexity library in c++, Universitat Ramon Llull, La Salle 196 (2010) 1–40. [[Link]](https://github.com/nmacia/dcol/blob/master/Documentation/Documentation.pdf)

<span id="Lorena2019">`[Lorena2019]`</span>
A. C. Lorena, L. P. Garcia, J. Lehmann, M. C. Souto, T. K. Ho, How complex is your classification problem? a survey on measuring classification complexity, ACM Computing Surveys (CSUR) 52 (5) (2019) 1–34. [[Link]](https://dl.acm.org/doi/abs/10.1145/3347711)

<span id="Barella2018">`[Barella2018]`</span>
V. H. Barella, L. P. Garcia, M. P. de Souto, A. C. Lorena, A. de Carvalho, Data complexity measures for imbalanced classification tasks, in: 2018 International Joint Conference on Neural Networks (IJCNN), IEEE, 2018, pp. 1–8. [[Link]](https://ieeexplore.ieee.org/document/8489661)

<span id="Garcia2020">`[Garcia2020]`</span>
L. P. Garcia, A. Rivolli, E. Alcoba ̧ca, A. C. Lorena, A. C. de Carvalho, Boosting meta-learning with simulated data complexity measures, Intelligent Data Analysis 24 (5) (2020) 1011–1028. [[Link]](https://content.iospress.com/articles/intelligent-data-analysis/ida194803)

<span id="Alcobaca2020">`[Alcobaca2020]`</span>
E. Alcobaça, F. Siqueira, A. Rivolli, L. P. F. Garcia, J. T. Oliva, A. C. P. L. F. de Carvalho, Mfe: Towards reproducible meta-feature extraction, Journal of Machine Learning Research 21 (111) (2020) 1–5. [[Link]](https://www.jmlr.org/papers/volume21/19-348/19-348.pdf)


<span id="Smith2014">`[Smith2014]`</span>
M. R. Smith, T. Martinez, C. Giraud-Carrier, An instance level analysis of data complexity, Machine learning 95 (2) (2014) 225–256. [[Link]](https://link.springer.com/article/10.1007/s10994-013-5422-z)

<span id="Kovacs2019">`[Kovacs2019]`</span>
G. Kovács, An empirical comparison and evaluation of minority oversampling techniques on a large number of imbalanced datasets, Applied Soft Computing 83 (2019). [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S1568494619304429)

<span id="Grycza2020">`[Grycza2020]`</span>
J. Grycza, D. Horna, H. Klimczak, K. Plucínski, Multi-imbalance:  Python package for multi-class imbalance learning, Poznan University of Technology, Poland, 2020. [[Link]](http://www.cs.put.poznan.pl/mlango/publications/multiimbalance/)

<span id="Douzas2017">`[Douzas2017]`</span>
G. Douzas, F. Bacao, Self-Organizing Map Oversampling (SOMO) for imbalanced data set learning, Expert systems with Applications 82 (2017): 40-52. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0957417417302324?via%3Dihub)

<span id="Douzas2018">`[Douzas2018]`</span>
G. Douzas, F. Bacao, F. Last, Improving imbalanced learning through a heuristic oversampling method based on k-means and SMOTE, Information Sciences 465 (2018): 1-20. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0020025518304997?via%3Dihub)

<span id="Zhang2019">`[Zhang2019]`</span>
C. Zhang, J. Bi, S. Xu, E. Ramentol, G. Fan, B. Qiao, H. Fujita, Multi-imbalance: An open-source software for multi-class imbalance learning. Knowledge-Based Systems, 174, 137-143, 2019. [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0950705119301042)