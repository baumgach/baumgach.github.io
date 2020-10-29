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

I am currently working on the four research areas below. 

### Safety and uncertainty

In medical image analysis, confidently predicting something false can have devastating consequences. Apart from achieving high predictive accuracy, one needs to establish the circumstances under which algorithmic predictions generalize, or give appropriate error bounds. This is highly relevant to patient safety and the regulation of machine learning based medical software. The goal in this branch, is develop deep learning methods founded in probability theory that can be used to estimate uncertainty stemming from sources such as the image reconstruction, or inherent limitations of an imaging modality.

#### Selected publications

 * **Christian F Baumgartner**, Kerem C Tezcan, Krishna Chaitanya, Andreas M Hötker, Urs J Muehlematter, Khoschy Schawkat, Anton S Becker, Olivio Donati, Ender Konukoglu., [Phiseg: Capturing uncertainty in medical image segmentation](https://arxiv.org/pdf/1906.04045.pdf), Proc. MICCAI 2019
 * Kerem C Tezcan, **Christian F Baumgartner**, Ender Konukoglu, [Sampling possible reconstructions of undersampled acquisitions in MR imaging](https://arxiv.org/abs/2010.00042), arXiv preprint arXiv:2010.00042 (2020)
 * Esther Puyol-Antón, Bram Ruijsink, **Christian F Baumgartner**, Pier-Giorgio Masci, Matthew Sinclair, Ender Konukoglu, Reza Razavi, Andrew P King, [Automated quantification of myocardial tissue characteristics from native T 1 mapping using neural networks with uncertainty-based quality-control](https://link.springer.com/article/10.1186/s12968-020-00650-y), Journal of Cardiovascular Magnetic Resonance (2020)

### Learning efficiently with fewer data

Obtaining annotated data is very expensive in the medical field because only clinical professionals can do it. In a first step this raises the question: how can we learn with fewer data, while still achieving acceptable performance. Annotation effort can be reduced by either only partially annotating each image (weakly supervised learning) or, alternatively, by only annotating a subset of images (semi-supervised learning). Different tasks may benefit from different annotation strategies.

#### Selected publications

 * Yigit B Can, Krishna Chaitanya, Basil Mustafa, Lisa M Koch, Ender Konukoglu, **Christian F Baumgartner**, [Learning to segment medical images with scribble-supervision alone](https://arxiv.org/pdf/1807.04668), Proc. DLMIA 2018
 * **Christian F Baumgartner**, Konstantinos Kamnitsas, Jacqueline Matthew, Tara P Fletcher, Sandra Smith, Lisa M Koch, Bernhard Kainz, Daniel Rueckert, [SonoNet: real-time detection and localisation of fetal standard scan planes in freehand ultrasound](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7974824), IEEE Transactions in Medical Imaging (2017)
 * Krishna Chaitanya, Neerav Karani, **Christian F Baumgartner**, Anton Becker, Olivio Donati, Ender Konukoglu, [Semi-supervised and task-driven data augmentation](https://arxiv.org/pdf/1902.05396), Proc. IPMI 2019
 * Lisa Margret Koch, Martin Rajchl, Wenjia Bai, **Christian F Baumgartner**, Tong Tong, Jonathan Passerat-Palmbach, Paul Aljabar, Daniel Rueckert, [Multi-atlas segmentation using partially annotated data: methods and annotation strategies](https://ieeexplore.ieee.org/iel7/34/8371350/08014481.pdf), Transactions in Pattern Recognition and Machine Intelligence (2017)

### Exploiting shared information between tasks

Humans learn new tasks by heavily relying on previous experiences. A doctor in training will learn to segment a previously unseen pathology in brain MR images by making use of their knowledge of similar pathologies, human anatomy, and the contrast properties of a certain imaging modality. They will be able to perform well on the task after seeing a very small number of examples. In contrast, current ML technologies for the most part leverage a large amount of training data to learn each task individually and from scratch. How can we teach machines to take advantage of similarities between tasks? Can we teach machines to implicitly or explicitly take advantage of common factors such as anatomy (a heart is still a heart in CT, as well as, MRI) or imaging modality?

*[MRI]: Magnetic Resonance imaging
*[CT]: Computed (X-ray) Tomography

#### Selected publications

 * Neerav Karani, Krishna Chaitanya, **Christian F Baumgartner**, Ender Konukoglu, [A lifelong learning approach to brain MR segmentation across scanners and protocols](https://arxiv.org/pdf/1805.10170), Proc. MICCAI 2018
 * Konstantinos Kamnitsas, **Christian F Baumgartner**, Christian Ledig, Virginia Newcombe, Joanna Simpson, Andrew Kane, David Menon, Aditya Nori, Antonio Criminisi, Daniel Rueckert, Ben Glocker, [Unsupervised domain adaptation in brain lesion segmentation with adversarial networks](https://arxiv.org/pdf/1612.08894), Proc. IPMI 2017

### Discovering effects in big medical data

Data is the most precious resource in our profession. Having realised this, many governments and organisations started collecting
massive and incredibly detailed datasets of patients suffering from diseases as well as healthy people. Some examples of such datasets are the [UK Biobank](https://www.ukbiobank.ac.uk/), the [German National Cohort Study](https://www.klinikum.uni-heidelberg.de/radiologische-klinik/klinik-fuer-diagnostische-und-interventionelle-radiologie/forschung/research-projects/the-german-national-cohort), or the [Alzheimer's Disease Neuroimaging Initiative](http://adni.loni.usc.edu/). These dataset contain not only images, but vast amounts of extra information such as genetic markers and life-style choices. In parallel, machine learning technology, in particular the fields of generative modelling and causal inference have progressed to a point where analysing such datasets on a pixel/voxel level becomes feasible. This creates an unprecedented opportunity to discover physiological mechanisms, disease processes, and connections between imaging and non-imaging data.

#### Selected publications

**Christian F Baumgartner**, Lisa M Koch, Kerem Can Tezcan, Jia Xi Ang, Ender Konukoglu, [Visual feature attribution using Wasserstein GANs](http://openaccess.thecvf.com/content_cvpr_2018/papers/Baumgartner_Visual_Feature_Attribution_CVPR_2018_paper.pdf), Proc. CVPR 2018

## Research Ethics

I strongly believe in:

 * Open publishing
 * Papers with code
 * Diversity in research
 * Slowing down the research cycle
