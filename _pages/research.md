---
permalink: /research/
title: "Research Interests"
author_profile: true
redirect_from:
  - /research.html
---

## What motivates me

Ultimately, the goal of medical image analysis driven by machine learning is to
obtain better patient outcomes. However, even though tremendous progress has been made
in research settings, surprisingly little of this technology has leaked into
medical practice. One reason for this is that the medical domain is an
extremely high-stakes application field with extraordinary demands on robustness
of algorithms. A further complication is that it is very difficult and expensive to prove
that the algorithms behave as intended to overseeing bodies such as the
[US FDA](https://en.wikipedia.org/wiki/Food_and_Drug_Administration) or the
[TÜVs](https://en.wikipedia.org/wiki/Technischer_%C3%9Cberwachungsverein).
On the other hand, doctors must be willing to use this technology and it must
be integrated into clinical workflows in a useful way, a problem often not
considered in pure research settings.

I want to develop technologies that help bridge this gap
between research and clinical practice. I believe two broad avenues to achieve
this are:
1. Developing machine learning methods that are founded in theory will allow us
to develop more robust algorithms, to better appreciate confidence bounds of
predictive algorithms, and to understand the relationship between training data
and algorithm performance. This will ultimately lead to algorithms that are more useful
and easier to certify.
2. Develop human-in-the-loop techniques, which optimally communicate prediction uncertainty,
and allow the operator to interact with the algorithm during the prediction and
training phase, in a life long learning setting.

## Specific research areas

### Safety and uncertainty

In medical image analysis, confidently predicting something false can have devastating consequences. Apart from achieving high predictive accuracy, one needs to establish the circumstances under which algorithmic predictions generalize, or give appropriate error bounds. This is highly relevant to patient safety and the regulation of machine learning based medical software. In my research, I develop deep learning methods founded in probability theory that can be used to estimate uncertainty stemming from sources such as the image reconstruction, or inherent limitations of an imaging modality.

#### Relevant papers

 * **Christian F Baumgartner**, Kerem C Tezcan, Krishna Chaitanya, Andreas M Hötker, Urs J Muehlematter, Khoschy Schawkat, Anton S Becker, Olivio Donati, Ender Konukoglu.; [Phiseg: Capturing uncertainty in medical image segmentation](https://arxiv.org/pdf/1906.04045.pdf), Proc. MICCAI 2019
 * Kerem C Tezcan, **Christian F Baumgartner**, Ender Konukoglu; [Sampling possible reconstructions of undersampled acquisitions in MR imaging](https://arxiv.org/abs/2010.00042), arXiv preprint arXiv:2010.00042 (2020)
 * Esther Puyol-Antón, Bram Ruijsink, **Christian F Baumgartner**, Pier-Giorgio Masci, Matthew Sinclair, Ender Konukoglu, Reza Razavi, Andrew P King [Automated quantification of myocardial tissue characteristics from native T 1 mapping using neural networks with uncertainty-based quality-control](https://link.springer.com/article/10.1186/s12968-020-00650-y), Journal of Cardiovascular Magnetic Resonance (2020)

### Learning efficiently with fewer data

Obtaining annotated data is very expensive in the medical field because only clinical professionals can do it. How can we learn with fewer data, and how can we obtain training data that are optimal for a certain task?

### Exploiting shared information between tasks

Often algorithms are learned from scratch for each new problem. Taking into account that many problems are related in various ways can help us create more intelligent algorithms.

### Discovering effects in big medical data

Recent advances in probabilistic machine learning techniques offer a unique opportunity to explore datasets with ten thousands of images (such as the [German National Cohort Study](https://www.klinikum.uni-heidelberg.de/radiologische-klinik/klinik-fuer-diagnostische-und-interventionelle-radiologie/forschung/research-projects/the-german-national-cohort)) to better understand disease processes.
