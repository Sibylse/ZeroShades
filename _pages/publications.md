---
title:  "Publications"
layout: archive
permalink: /pubs/
author_profile: true
comments: false
---

## Journal Publications:
<details>
  <summary>
    BROCCOLI: overlapping and outlier-robust biclustering through proximal stochastic gradient descent <br>
    <i>Sibylle Hess, Gianvito Pio, Michiel Hochstenbach, and Michelangelo Ceci @ Data Mining and Knowledge Discovery (DAMI) 2021</i>
  </summary>
  <p>
  Broccoli extends the numerical optimization used for Boolean matrix factorizations (cf. <i>the Primping routine, the Trustworthy Pal</i> and <i>C-Salt</i>) to biclusterings. The biclustering model is a tri-factorization of the data into two outer binary matrices indicating observation- and feature-clusters and a middle real-valued matrix, called the core matrix. Unlike in Boolean matrix factorization, the biclustering tri-factorization does not require the approximation of the matrix product in another algebra. We have exploited this fact with our optimization objective, which follows (like our Boolean matrix factorization optimization schemes) the penalized approach, where the binary constraints are relaxed but nonbinary values are penalized. However, the proposed objective optimizes not only the factor matrices, but also the penalization weights. This way, the penalization weights gradually increase throughout the optimization - arriving at binary matrices at convergence. 
   </p>
</details>
[publication](https://link.springer.com/article/10.1007/s10618-021-00787-z){: .btn .btn--success .btn--small} [Pytorch code](https://github.com/Sibylse/Broccoli){: .btn .btn--warning .btn--small} [talk](https://recorder-v3.slideslive.com/?share=47344&s=23dbd1bf-d84e-4cb2-8d58-5d40ce599895){: .btn .btn--info .btn--small}

<details>
  <summary>
    The PRIMPING routine — Tiling through proximal alternating linearized minimization <br>
    <i>Sibylle Hess, Katharina Morik, and Nico Piatkowski @ Data Mining and Knowledge Discovery (DAMI) 2022</i>
  </summary>
  <p>
  The Primping Routine introduces a novel optimization procedure for the combinatorial problem of Boolean Matrix Factorization (BMF), based on recent advances in nonconvex optimization. The proposed procedure has been the first to enable the highly parallel implementation of a BMF algorithm on Graphics Processing Units (GPUs), replacing the so far used heuristic procedures. Furthermore, a minimum description length based criterion is introduced which enables an accurate automatic determination of the number of clusters. The introduced proximal operator for binary optimization has been extended for integer optimization in the scope of estimating exponential families 
<a href="https://eldorado.tu-dortmund.de/bitstream/2003/36877/1/Dissertation_Piatkowski.pdf">(Piatkowski, 2018)</a>.
   </p>
</details>
[arXiV](https://arxiv.org/abs/1906.09722){: .btn .btn--primary .btn--small} [publication](https://link.springer.com/article/10.1007/s10618-017-0508-z){: .btn .btn--success .btn--small} [C++ code](https://bitbucket.org/np84/paltiling/src/master/){: .btn .btn--warning .btn--small}

## Conference Publications:
<details>
  <summary> 
    Scoring Rule Nets: Beyond Mean Target Prediction in Multivariate Regression <br>
    <i>Daan Roordink, Sibylle Hess, Katharina Morik @ ECML PKDD 2023</i>
  </summary>
  <p>
    We propose a new multivariate scoring rule, the Conditional Continuous Ranked Probability Score (CCRPS) which is a multivariate strictly proper scoring rule that extends on the Continuous Ranked Probability Score (CRPS). Scoring rules can be seen as loss functions that incorporates calibration and precision of a probabilistic prediction. Hence, scoring rules fidn application among other things in probabilistic regression. A standard way to train probabilistic regression models is to use a maximum likelihood estimation (MLE). However, MLE sometimes overestimate variance to an unacceptable degree. This is particularly a problem in the multivariate domain, and univariate models often optimize the CRPS. Yet, in the multivariate domain, no such alternative to MLE has yet been widely accepted. The Energy Score – the most investigated alternative – notoriously lacks closed-form expressions and sensitivity to the correlation between target variables. In response, we propose Conditional CRPS, for which we prove desirable theoretical properties, such as strict propriety. We show that closed-form expressions exist for popular distributions and illustrate their sensitivity to correlation. We then show in a variety of experiments on both synthetic and real data, that Conditional CRPS often outperforms MLE, and produces results comparable to state-of-the-art non-parametric models, such as Distributional Random Forest (DRF).
  </p>
</details>
[arXiV](https://arxiv.org/abs/2409.14456){: .btn .btn--primary .btn--small} [publication](https://link.springer.com/chapter/10.1007/978-3-031-43415-0_12){: .btn .btn--success .btn--small} [Tensorflow code](https://github.com/DaanR/scoringrule_networks){: .btn .btn--warning .btn--small} 
<details>
  <summary> 
    Shrub Ensembles for Online Classification <br>
    <i>Sebastian Buschjäger, Sibylle Hess, Katharina Morik @ AAAI 2022</i>
  </summary>
  <p>
    We apply proximal optimization to learn an ensemble of small decision trees (called shrubs) in a streaming setting. With this approach, we are able to maintain the effectiveness of decision tree ensembles (being able to adapt to changes in the data) in a memory-efficient model. The amount of available memory can be steered by the maximum number of decision shrubs that compose the ensemble. The composition of the decision shrubs is learned via proximal optimization, which yields theoretically guaranteed optimality properties on the derived selection of shrubs. This makes our approach suitable for resource constrained applications. This is also reflected in our experimental evaluation, showing that our Shrub Ensembles retain an excellent performance even when only little memory is available. 
  </p>
</details>
[arXiV](https://arxiv.org/pdf/2112.03723.pdf){: .btn .btn--primary .btn--small} [publication](https://ojs.aaai.org/index.php/AAAI/article/view/20560){: .btn .btn--success .btn--small} [Python code](https://github.com/sbuschjaeger/se-online){: .btn .btn--warning .btn--small} 
<details>
  <summary> 
   k is the Magic Number — Inferring the Number of Clusters Through Nonparametric Concentration Inequalities <br>
    <i>Sibylle Hess, and Wouter Duivesteijn @ ECML PKDD 2019</i>
  </summary>
  <p>
    This paper extends the idea of <i>the trustworthy pal</i> to select clusters based on the probability that a cluster is generated by noise effects to 
    clusters in the real-valued vector space computed by <i>k</i>-means. Here, me and my co-author have proposed a bound on the question whether a 
    cluster is likely to be part of another, overarching cluster. For real-valued clustering, comparable probability bounds exist, but only for specific 
    (e.g., Gaussian) distributions of points within one cluster. Our novel bound does not require assumptions of specific probability distribution and 
    relies only on easily computed parameters of the data, such as the mean and variance of points within each cluster. This makes our novel approach 
    suitable for the application of clustering methods which work on a transformation of the input data such as <i>SpectACl</i>.
  </p>
</details>
[arXiV](https://arxiv.org/abs/1907.02343){: .btn .btn--primary .btn--small} [publication](https://link.springer.com/chapter/10.1007/978-3-030-46150-8_16){: .btn .btn--success .btn--small} [Python code](https://github.com/Sibylse/SpecialK){: .btn .btn--warning .btn--small}
<details>
  <summary> 
    The SpectACl of nonconvex clustering: a spectral approach to density-based clustering <br> 
    <i> Sibylle Hess, Wouter Duivesteijn, Philipp Honysz, and Katharina Morik @ AAAI 2019</i>
  </summary> 
  <p>
    This paper fills a long standing theoretical gap, showing why the application of <i>k</i>-means in Spectral Clustering is not only practically but also 
    theoretically justified. This insight led to the proposal of a novel robust and feasible algorithm <i>SpectACl</i>. <i>SpectACl</i> is able to 
    outperform more advanced and theoretically more expressive approaches which learn the similarity matrix simultaneously with the clustering.
  </p>
</details>
[arXiV](https://arxiv.org/abs/1907.00680){: .btn .btn--primary .btn--small} [publication](https://ojs.aaai.org/index.php/AAAI/article/view/4265){: .btn .btn--success .btn--small}
<details>
  <summary>
  The relationship of DBSCAN to matrix factorization and spectral clustering <br>
  <i>Erich Schubert, Sibylle Hess and Katharina Morik @ LWDA 2018 </i>
  </summary>
  <p>
  In this paper, we explore the not obvious relationships between the density-based clustering of DBSCAN and the minimum-cut based clustering by Spectral Clustering, which in turn can be formalized as a matrix factorization task. 
  </p>
</details>
[publication](http://ceur-ws.org/Vol-2191/paper38.pdf){: .btn .btn--success .btn--small}

<details>
  <summary>
    The trustworthy pal: Controlling the false discovery rate in boolean matrix factorization <br>
    <i> Sibylle Hess, Nico Piatkowski, and Katharina Morik @ SDM 2018 </i> 
  </summary>
  <p>
    In this paper, we provide the first criterion to determine the number of clusters in BMF based on probability theory. We have provided a
    probabilistic bound on the question "Given my data has <i>p\%</i> noise, how likely is this cluster (returned by my method of choice) mainly 
    composed of noise?". This approach certifies the returned clustering in the sense that any of the clusters is only with a small (user-defined)
    probability an artifact of noise.
  </p>
</details>
[arXiV](https://arxiv.org/abs/1907.00697){: .btn .btn--primary .btn--small} [publication](https://epubs.siam.org/doi/abs/10.1137/1.9781611975321.46){: .btn .btn--success .btn--small}  [C++ code and Julia script](https://bitbucket.org/Sibylse/trustpal/src/master/){: .btn .btn--warning .btn--small}
<details>
  <summary>C-salt: Mining class-specific alterations in boolean matrix factorization <br>
    <i>Sibylle Hess and Katharina Morik @ ECML PKDD </i>
  </summary>
    <p>
      <i>C-SALT</i> presents a novel matrix factorization scheme which reveals the clustering structure subject to given classes. 
      <i>C-Salt</i> provides  answers to the question: "Given samples of various classes in the binary feature space, what are the features 
      which define clusters stretching over multiple classes and how do these clusters change within a particular class?" 
      The optimization for the novel BMF scheme, answering this question, relies on the method established in the primping routine. 
      <i>C-Salt</i> has proven particularly useful in the application of medical domains. The development of personalised medicine requires models 
      which can do both: identifying groups of patients, sharing  genomic traits, together with the alterations of these traits which discriminate 
      those developing a particular disease from those who do not.
  </p>
 </details>
[arXiV](https://arxiv.org/abs/1906.09907){: .btn .btn--primary .btn--small} [publication](https://link.springer.com/chapter/10.1007/978-3-319-71249-9_33){: .btn .btn--success .btn--small} [C++ code](https://bitbucket.org/Ilsebyl/c-salt/src/master/){: .btn .btn--warning .btn--small}

<details>
  <summary>
    SHrimp: Descriptive Patterns in a Tree <br>
    <i>Sibylle Hess, Nico Piatkowski and Katharina Morik @ LWDA 2014 </i>
  </summary>
  My first paper, submitted before I got my diploma in Computer Science. It's proposing an efficient tree-structure to traverse a set of frequent itemsets, in order to decide quickly if a candidate itemset could be interesting or not. Interestingness is hereby defined by the information-theoretic measure of interestingness known from the method <i>Krimp</i>. 
</details>
[publication](https://pure.tue.nl/ws/files/125071574/paper30.pdf){: .btn .btn--success .btn--small}

## Books/Chapters
<details>
  <summary>
    Chapter: Matrix Factorization with Binary Constraints @ Machine Learning under Resource Constraints - Volume 1: Fundamentals<br>
    <i>Sibylle Hess, 2022</i>
  </summary>
  <p>I wrote a chapter in this series of books that highlight the results of the three funded periods of the <a> href="https://sfb876.tu-dortmund.de/index.html">SFB 876</a>@TU Dortmund. The chapter summarizes and shortly surveys strategies in optimization subject to binary constraints in the scope of clustering objectives that are based on matrix factorization.</p>
</details>
[publication](https://doi.org/10.1515/9783110785944-005){: .btn .btn--success .btn--small}
<details>
  <summary>
    A Mathematical Theory of Making Hard Decisions: Model Selection and Robustness of Matrix Factorization with Binary Constraints <br>
    <i>Sibylle Hess, 2019</i>
  </summary>
  <p>This is my dissertation which contains a survey about matrix factorizations subject to binary constraints and the connections to popular clustering methods. In this scope, I present my work on the <i>Primping Routine</i>, <i>Spectacl</i>, <i>The Trustworthy Pal</i> and <i>C-Salt</i>. Big shout-out to the <a> href="https://sfb876.tu-dortmund.de/index.html">SFB 876</a>@TU Dortmund and my supervisor Katharina Morik.</p>
</details>
[publication](https://eldorado.tu-dortmund.de/bitstream/2003/38270/1/DissHess.pdf){: .btn .btn--success .btn--small}
