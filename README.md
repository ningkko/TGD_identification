# Identification of transgender and gender diverse individuals in electronic health records

This work was presented at the AMIA Annual Symposium 2022 and ICHI 2023.

This paper is published in the Journal of Biomedical Informatics. If you use the dictionary, kindly cite us with
```
@article{HUA2023104507,
title = {A deep learning approach for transgender and gender diverse patient identification in electronic health records},
journal = {Journal of Biomedical Informatics},
pages = {104507},
year = {2023},
issn = {1532-0464},
doi = {https://doi.org/10.1016/j.jbi.2023.104507},
url = {https://www.sciencedirect.com/science/article/pii/S1532046423002289},
author = {Yining Hua and Liqin Wang and Vi Nguyen and Meghan Rieu-Werden and Alex McDowell and David W. Bates and Dinah Foer and Li Zhou},
keywords = {Gender Identity, Transgender Persons, Sexual and Gender Minorities, Electronic Health Records, Machine Learning, Natural Language Processing},
abstract = {Background
Although accurate identification of gender identity in the electronic health record (EHR) is crucial for providing equitable health care, particularly for transgender and gender diverse (TGD) populations, it remains a challenging task due to incomplete gender information in structured EHR fields.
Objective
Using TGD identification as a case study, this research uses NLP and deep learning to build an accurate patient gender identity predictive model, aiming to tackle the challenges of identifying relevant patient-level information from EHR data and reducing annotation work.
Methods
This study included adult patients in a large healthcare system in Boston, MA, between 4/1/2017 to 4/1/2022. To identify relevant information from massive clinical notes and to denoise, we compiled a list of gender-related keywords through expert curation, literature review, and expansion via a fine-tuned BioWordVec model. This keyword list was used to pre-screen potential TGD individuals and create two datasets for model training, testing, and validation. Dataset I was a balanced dataset that contained clinician-confirmed TGD patients and cases without keywords. Dataset II contained cases with keywords. The performance of the deep learning model was compared to traditional machine learning and rule-based algorithms.
Results
The final keyword list consists of 109 keywords, of which 58 (53.2%) were expanded by the BioWordVec model. Dataset I contained 3,150 patients (50% TGD) while Dataset II contained 200 patients (90% TGD). On Dataset I the deep learning model achieved a F1 score of 0.917, sensitivity of 0.854, and a precision of 0.980; and on Dataset II a F1 score of 0.969, sensitivity of 0.967, and precision of 0.972. The deep learning model significantly outperformed rule-based algorithms.
Conclusion
This is the first study to show that deep learning-integrated NLP algorithms can accurately identify gender identity using EHR data. Future work should leverage and evaluate additional diverse data sources to generate more generalizable algorithms.}
}
```
