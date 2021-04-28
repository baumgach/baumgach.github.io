---
permalink: /research/
title: "Research motivation"
author_profile: true
redirect_from:
  - /research.html
---

In the field of medical image analysis, the ultimate goal is to improve patient
outcomes. There are a number of broad ways in which machine learning can help achieve this goal:
 - Relieving the burden on doctors and the healthcare system by accelerating and simplifying the analysis of medical images through partial or full automation of steps such as diagnosis, outcome prediction, image quantification, and image reconstruction.
 - Developing technology which enables completely novel clinical workflows which are not possible without AI support.
 - Extraction of new clinical knowledge from large image data bases, which can inform future clinical dectisions, treatments and drug trials.

However, even though tremendous progress has been made for all of those points in research settings,
surprisingly little of this technology has leaked into
medical practice. One reason for this is that the medical domain is an
extremely high-stakes application field with extraordinary demands on robustness
of algorithms. Another reason is that algorithmic outputs are not suitable for clinical decision making if neither the patient nor the doctor can understand the reasoning behind the prediction, and clinicians are loath to use the thus-far predominately black-box technology. Both of the above points also have important implications for the certification of AI technology.

Therefore, in order to start harnessing the massive potential of machine learning
for healthcare, and to actually use it to improve real patient outcomes,
I aim to do research that helps to bridge this gap between machine learning and
clinical practice.

Specific research areas
======

Safety and uncertainty
------

In medical image analysis, confidently predicting something false can have devastating consequences. Apart from achieving high predictive accuracy, one needs to establish the circumstances under which algorithmic predictions generalize, or give appropriate error bounds. This is highly relevant to patient safety and the regulation of machine learning based medical software. The goal in this branch, is develop deep learning methods founded in probability theory that can be used to estimate uncertainty stemming from sources such as the image reconstruction, or inherent limitations of an imaging modality.

**Selected publications**

 * **Christian F Baumgartner**, Kerem C Tezcan, Krishna Chaitanya, Andreas M Hötker, Urs J Muehlematter, Khoschy Schawkat, Anton S Becker, Olivio Donati, Ender Konukoglu., [Phiseg: Capturing uncertainty in medical image segmentation](https://arxiv.org/pdf/1906.04045.pdf), Proc. MICCAI 2019
 * Kerem C Tezcan, **Christian F Baumgartner**, Ender Konukoglu, [Sampling possible reconstructions of undersampled acquisitions in MR imaging](https://arxiv.org/abs/2010.00042), arXiv preprint arXiv:2010.00042 (2020)
 * Esther Puyol-Antón, Bram Ruijsink, **Christian F Baumgartner**, Pier-Giorgio Masci, Matthew Sinclair, Ender Konukoglu, Reza Razavi, Andrew P King, [Automated quantification of myocardial tissue characteristics from native T 1 mapping using neural networks with uncertainty-based quality-control](https://link.springer.com/article/10.1186/s12968-020-00650-y), Journal of Cardiovascular Magnetic Resonance (2020)


Interpretable machine learning
------
The rapid developments and early successes of deep learning technology in medical image analysis (and other fields) have caused the field to prioritise predictive accuracy over human integration. However, it is becoming increasingly clear that black box models are unlikely to find clinical acceptance, can lead to ethical problems when neither the patient nor the doctor understand the reasoning behind a prediction, and are difficult to certify. Our research goals in this branch are to develop adequate explanations for predictions of deep learning models, and perhaps more importantly, to build inherently interpretable models rooted in prior clinical knowledge.

**Selected publications**

 * **Christian F Baumgartner**, Konstantinos Kamnitsas, Jacqueline Matthew, Tara P Fletcher, Sandra Smith, Lisa M Koch, Bernhard Kainz, Daniel Rueckert, [SonoNet: real-time detection and localisation of fetal standard scan planes in freehand ultrasound](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7974824), IEEE Transactions in Medical Imaging (2017)


Human-in-the-loop systems
------
Humans are not only involved in obtaining the final prediction of a machine learning based system. Especially in medical contexts, human users are also involved in collecting and annotating the training data, and in continuously improving the model over time by adding particularly informative cases to the model. What is more, those steps can often only be performed by clinicians who often need to perform these tasks working after hours in addition to their clinical responsibilities. To address these topics we investigate optimizing annotation time by using weak and active learning techniques. In addition to placing humans in the training loop, for some applications humans must also be placed in the prediction loop. For instance the initial prediction of an algorithm, e.g. an organ delineation task or a radiotherapy plan, may not completely agree with the users expectations. The clinician may want to refine her query for the algorithm and obtain an improved prediction. How to integrate humans into the prediction loop is studied in the field of interactive learning.

**Selected publications**

 * Yigit B Can, Krishna Chaitanya, Basil Mustafa, Lisa M Koch, Ender Konukoglu, **Christian F Baumgartner**, [Learning to segment medical images with scribble-supervision alone](https://arxiv.org/pdf/1807.04668), Proc. DLMIA 2018
 * Krishna Chaitanya, Neerav Karani, **Christian F Baumgartner**, Anton Becker, Olivio Donati, Ender Konukoglu, [Semi-supervised and task-driven data augmentation](https://arxiv.org/pdf/1902.05396), Proc. IPMI 2019
 * Lisa Margret Koch, Martin Rajchl, Wenjia Bai, **Christian F Baumgartner**, Tong Tong, Jonathan Passerat-Palmbach, Paul Aljabar, Daniel Rueckert, [Multi-atlas segmentation using partially annotated data: methods and annotation strategies](https://ieeexplore.ieee.org/iel7/34/8371350/08014481.pdf), Transactions in Pattern Recognition and Machine Intelligence (2017)


Discovering effects in big medical data
------

Data is the most precious resource in our profession. Having realised this, many governments and organisations started collecting
massive and incredibly detailed datasets of patients suffering from diseases as well as healthy people. Some examples of such datasets are the [UK Biobank](https://www.ukbiobank.ac.uk/), the [German National Cohort Study](https://www.klinikum.uni-heidelberg.de/radiologische-klinik/klinik-fuer-diagnostische-und-interventionelle-radiologie/forschung/research-projects/the-german-national-cohort), or the [Alzheimer's Disease Neuroimaging Initiative](http://adni.loni.usc.edu/). These dataset contain not only images, but vast amounts of extra information such as genetic markers and life-style choices. In parallel, machine learning technology, in particular the fields of generative modelling and causal inference have progressed to a point where analysing such datasets on a pixel/voxel level becomes feasible. This creates an unprecedented opportunity to discover physiological mechanisms, disease processes, and connections between imaging and non-imaging data. A focus of our group is to develop scalable probabilistic modelling and inference techniques to analyse such data.

**Selected publications**

**Christian F Baumgartner**, Lisa M Koch, Kerem Can Tezcan, Jia Xi Ang, Ender Konukoglu, [Visual feature attribution using Wasserstein GANs](http://openaccess.thecvf.com/content_cvpr_2018/papers/Baumgartner_Visual_Feature_Attribution_CVPR_2018_paper.pdf), Proc. CVPR 2018


<!-- Past research
======

Learning efficiently with fewer data
------

Obtaining annotated data is very expensive in the medical field because only clinical professionals can do it. In a first step this raises the question: how can we learn with fewer data, while still achieving acceptable performance. Annotation effort can be reduced by either only partially annotating each image (weakly supervised learning) or, alternatively, by only annotating a subset of images (semi-supervised learning). Different tasks may benefit from different annotation strategies.

**Selected publications**

 * Yigit B Can, Krishna Chaitanya, Basil Mustafa, Lisa M Koch, Ender Konukoglu, **Christian F Baumgartner**, [Learning to segment medical images with scribble-supervision alone](https://arxiv.org/pdf/1807.04668), Proc. DLMIA 2018
 * **Christian F Baumgartner**, Konstantinos Kamnitsas, Jacqueline Matthew, Tara P Fletcher, Sandra Smith, Lisa M Koch, Bernhard Kainz, Daniel Rueckert, [SonoNet: real-time detection and localisation of fetal standard scan planes in freehand ultrasound](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7974824), IEEE Transactions in Medical Imaging (2017)
 * Krishna Chaitanya, Neerav Karani, **Christian F Baumgartner**, Anton Becker, Olivio Donati, Ender Konukoglu, [Semi-supervised and task-driven data augmentation](https://arxiv.org/pdf/1902.05396), Proc. IPMI 2019
 * Lisa Margret Koch, Martin Rajchl, Wenjia Bai, **Christian F Baumgartner**, Tong Tong, Jonathan Passerat-Palmbach, Paul Aljabar, Daniel Rueckert, [Multi-atlas segmentation using partially annotated data: methods and annotation strategies](https://ieeexplore.ieee.org/iel7/34/8371350/08014481.pdf), Transactions in Pattern Recognition and Machine Intelligence (2017)

Exploiting shared information between tasks
------

Humans learn new tasks by heavily relying on previous experiences. A doctor in training will learn to segment a previously unseen pathology in brain MR images by making use of their knowledge of similar pathologies, human anatomy, and the contrast properties of a certain imaging modality. They will be able to perform well on the task after seeing a very small number of examples. In contrast, current ML technologies for the most part leverage a large amount of training data to learn each task individually and from scratch. How can we teach machines to take advantage of similarities between tasks? Can we teach machines to implicitly or explicitly take advantage of common factors such as anatomy (a heart is still a heart in CT, as well as, MRI) or imaging modality?

*[MRI]: Magnetic Resonance imaging
*[CT]: Computed (X-ray) Tomography

**Selected publications**

 * Neerav Karani, Krishna Chaitanya, **Christian F Baumgartner**, Ender Konukoglu, [A lifelong learning approach to brain MR segmentation across scanners and protocols](https://arxiv.org/pdf/1805.10170), Proc. MICCAI 2018
 * Konstantinos Kamnitsas, **Christian F Baumgartner**, Christian Ledig, Virginia Newcombe, Joanna Simpson, Andrew Kane, David Menon, Aditya Nori, Antonio Criminisi, Daniel Rueckert, Ben Glocker, [Unsupervised domain adaptation in brain lesion segmentation with adversarial networks](https://arxiv.org/pdf/1612.08894), Proc. IPMI 2017 -->


Research ethics
======

I strongly believe in:

 * Open publishing
 * Papers with code
 * Diversity in research
 * Slowing down the publishing cycle
