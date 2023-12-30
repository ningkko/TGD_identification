# A deep learning approach for transgender and gender diverse patient identification in electronic health records
DOI: [https://doi.org/10.1016/j.jbi.2023.104507](https://doi.org/10.1016/j.jbi.2023.104507)

### Keywords generated from literature review, expert knowledge, and BioWordVec:
Table 1. TGD-related Keyword Lists Source

| Keywords List                                 | Source                               |
|----------------------------------------------|--------------------------------------|
| Keyword list I (clinician-curated)           | - \bF to M\b, \bM to F\b, binary titles, bottom surgery, female to male, gender change, gender dysphoria, gender identity disorder, gender reassignment, gender surgery, gender transition, genderqueer, male to female, male-to-female, non binary, non-binary, nonbinary, sex change, sex reassignment, top surgery, trans female, trans male, trans-gender, transfeminine, transgender, transmasculine, transsexual |
| Keyword list II (identified from literature)  | - Roblin et al. (2016): Female-to-male, gender dysphoria, gender identity disorder, gender reassignment, male-to-female, sex reassignment, trans-gender, transsexual, transvest |
|                                              | - Xie et al. (2021): Female to male, gender change, gender dysphoria, gender identity disorder, gender reassignment, gender transformation, male to female, sex change, sex reassignment, sex transformation, transgender, transition to female, transition to male, transsexual, transvest |
|                                              | - Guo et al. (2021): \bF to M\b, \bgay\b, \bM to F\b, agender, ambiguous genitalia, assigned female, assigned gender, assigned male, assigned sex, bigender, binary titles, binary trans, biological female, biological male, biologically female, biologically male, birth sex, bottom surgery, breast augmentation, changed name, chest binding, cross dress, cross gender, cross sex, crossdress, dead name, deadname, demifemale, demimale, desired gender, female to male, female-to-male, male to female, male-to-female, trans-sexual, transsexual |
| Keyword list III (combined and expanded)      | The main list: \bF to M\b, \bM to F\b, agender, assigned female, assigned gender, assigned male, assigned sex, binary trans, biological female, biological male, biologically female, biologically male , birth sex, cross gender, cross sex, dead name, deadname, desired gender, female to male, female-to-male*, feminization*, feminizing hormone therapy*, feminizing vaginoplasty*, gender affirm*, gender assigned*, gender binary*, gender change, gender confirmation*, gender creative*, gender disorder*, gender dysphoria, gender fluid*, gender identity disorder, gender identity issues*, gender identity uncertain*, gender incongruence*, gender issues*, gender neutral*, gender non-conform*, gender nonconform*, gender presentation*, gender pronoun*, gender queer*, gender reassignment, gender surgery, gender transition, genderfluid*, genderqueer, hormonal transition*, intersex*, male to female, male-to-female*, masculinization*, masculinizing hormone therapy*, misgender*, non binary, non-binary, nonbinary, null gender*, reassignment surgery*, sex change, sex reassignment, they/them*, theythem*,trans female, trans male, trans men*, trans people*, trans women*, trans-gender, transfeminine, transgender, transgender surgery*, transhealth*, transition to female, transition to male, transmasculine, transmen*, transsexual, transvest, transwomen* |
|                                              | The complementary list: ambiguous genitalia, augmentation mammoplasty*, bottom surgery, breast augmentation, changed name, chest binding, cross dress, crossdress, facial feminization*, gender expression*, gender unknown*, hysterectomy*, metoidioplasty*, orchiectomy*, permanent hair removal*, original birth*, preferred pronoun*, questioning gender*, sex unknown*, two spirit*, tomboy*, top surgery, unknown gender*, unknown sex*, vaginectomy*, vaginoplasty*, vocal feminization*, voice modification* |
| Abbreviations:                                | F to M, female to male; M to F, male to female. |
|                                              | * Expanded keywords from BioWordVec-TGD. |
|                                              | \b represents a leading/trailing whitespace. |
| Authors note:                                | As detailed in the methods, this list was compiled to include terminology that would maximally capture data from the sources used. As a result, this list contains terminology that is stigmatizing and outdated. |


### The workflow
![Workflow](https://github.com/ningkko/TGD_identification/blob/main/workflow.jpg)

### Notes
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
