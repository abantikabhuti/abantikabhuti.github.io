---
title: "Higgs Boson ML Challenge"
date: 2026-03-01
tags: ["Python","Binary Classification","EDA","XGBoost"]
categories: ["Machine Learning"]
externalUrl: 
draft: false
showTableOfContents : true
---
**This article is being updated.**
{{< katex >}}
> [!info] Project repository
> See the [Github repo](https://github.com/abantikabhuti/higgs-ml-challenge) for a detailed overview of my project.
## Introduction
The Higgs Machine Learning Challenge was an open data analysis competition that took place between May and September 2014. Samples of simulated data from the ATLAS Experiment at the LHC corresponding to signal events with Higgs bosons decaying to \(\tau^+\tau^-\) together with background events were made available to the public through the website of the data science organization **Kaggle**. Participants attempted to identify the search region in a space of 30 kinematic variables that would maximize the expected discovery significance of the signal process.[^1]
## Evaluation
The evaluation metric is the **approximate median significance (AMS)**:

$$\text{AMS} = \sqrt{2\left[(s + b + b_r)\ln\left(1 + \frac{s}{b + b_r}\right) - s \right]}$$

where

- \(s, b\) : unnormalized true positive and false positive rates, respectively,
- \(b_r=10\) is the constant regularization term,
- \(ln\) is the natural log.
## Links
> [!info] Links
> - See the official challenge and datasets as hosted on [Kaggle](https://www.kaggle.com/competitions/higgs-boson).
> - For more information on the statistical model and the derivation of the metric, see the [official technical documentation](https://higgsml.lal.in2p3.fr/files/2014/04/documentation_v1.8.pdf).
> - The extended version of the dataset can be found [here](https://opendata.cern.ch/record/328#:~:text=This%20dataset%20is%20an%20extended,Machine%20Learning%20Challenge%20on%20Kaggle).

[^1]: C Adam-Bourdarios et al 2015 J. Phys.: Conf. Ser. 664 072015


