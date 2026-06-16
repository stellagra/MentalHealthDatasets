# Mental Health Datasets

A curated collection of datasets for mental health research, covering mood disorders, psychosis-risk, neurodevelopmental conditions, infant/early development, and general affective computing resources across facial, audio, physiological, and multimodal modalities.


**Notes:**
This repo is under development. Feel free to reach out for additions and/or corrections. If you find a link or reference is outdated, I am happy to receive your feedback.

- I neither claim completeness nor correctness. No guarantees.
- Access rights to the databases might change or licenses might run out.
- I do not own any of the following databases. For questions about access and details, do NOT contact me! Reach out to the respective authors.


---

## Table of Contents

- [Notation](#notation)
- [Table Overview](#table-overview)
- [Depression](#depression)
- [Bipolar Disorder](#bipolar-disorder)
- [Schizophrenia & Psychosis](#schizophrenia--psychosis)
- [Autism & Neurodevelopmental Disorders](#autism--neurodevelopmental-disorders)
- [Anxiety & Stress](#anxiety--stress)
- [Infant & Early Development](#infant--early-development)
- [Suicide Risk & Crisis Intervention](#suicide-risk--crisis-intervention)
- [Multimodal and General Mental Health Resources](#multimodal-and-general-mental-health-resources)
- [Related Sources](#related-sources)
- [2DO](#2do)
- [Contact](#contact)


---

## Notation

### Availability 
Availability is indicated as follows:

- ✅ Free to download
- 📧 Free upon request (most are for academics only 🎓)
- 🔒 Not publicly available
- 💰 Payment required
- ❌ No longer available

### Modality Legend

| Symbol | Modality |
|:---:|---|
| 🎥 | Video (raw footage) |
| 🖼️ | Images (raw) |
| 📐 | Facial features / AUs (extracted, e.g. via OpenFace, PyAFAR) |
| 👁️ | Eye gaze / Eye tracking |
| 🎙️ | Audio (raw) |
| 📝 | Text / Transcripts |
| 🧠 | EEG |
| ⌚ | Wearable / Actigraphy |
| 📱 | Smartphone logs (calls, SMS) |
| 🦴 | Skeletal / Pose |
| 💓 | Physiological (HR, EDA) |

### Description (below)

Entries with details are listed as as follows

- name + link
  * short description
  * annotations: ...
  * reference: ...
  * available: ...



---

## Table Overview

| Dataset | Condition (Measure) | Modalities | N | Access |
|---|---|:---:|---|:---:|
| [DAIC-WOZ](https://dcapswoz.ict.usc.edu/) | Depression (PHQ-8), PTSD (PCL-C) | 📐 🎙️ 📝 | 189 sessions | 📧 |

---

## Depression

- [Distress Analysis Interview Corpus (DAIC)](https://aclanthology.org/L14-1421/)
  * The Distress Analysis Interview Corpus of human and computer interviews
  * annotations: PHQ-8 (depression), and more
  * reference: Gratch J, Artstein R, Lucas GM, Stratou G, Scherer S, Nazarian A, Wood R, Boberg J, DeVault D, Marsella S, Traum DR. The Distress Analysis Interview Corpus of Human and Computer Interviews. In Proceedings of LREC 2014 May (pp. 3123-3128).
  * ❌ available: does not seem to be available as a whole

- [DAIC-WOZ Database](https://dcapswoz.ict.usc.edu/)
  * Subset of the larger DAIC. Virtual interviewer. 189 sessions ranging 7–33 minutes (average 16 minutes). Contains features extracted from video (not actual footage), transcripts, participant audio, and facial expressions (FACS-encoded by OpenFace 2.0).
  * annotations: PHQ-8 all items (depression), gender
  * reference: DeVault, D., Artstein, R., Benn, G., et al. (2014). "SimSensei kiosk: A virtual human interviewer for healthcare decision support." In Proceedings of AAMAS'14, Paris.
  * 📧 available: upon request for academics

- [Extended DAIC Database](https://dcapswoz.ict.usc.edu/)
  * Extended version of DAIC-WOZ for depression and PTSD assessment; used in AVEC 2019.
  * reference: Ringeval, F., Schuller, B., Valstar, M., et al. "AVEC 2019 workshop and challenge: State-of-mind, detecting depression with AI, and cross-cultural affect recognition." ACM, 2019.
  * 📧 available: upon request for academics
  
- [Depresjon](https://datasets.simula.no/depresjon/) ([kaggle](https://www.kaggle.com/datasets/arashnic/the-depression-dataset)) (2018)
  * Motor activity recordings of 23 unipolar and bipolar depressed patients and 32 healthy controls.
  * annotations: depression episode labels, unipolar/bipolar distinction
  * reference: "A Motor Activity Database of Depression Episodes in Unipolar and Bipolar Patients"
  * ✅ available: free to download

- [The DepreST Call and Text (DepreST-CAT) Dataset](https://github.com/mltlachac/DepreST-CAT) ([project page](https://emutivo.wpi.edu/index.php/data/))
  * Call and text logs collected during COVID-19 pandemic. 369 Prolific crowd-sourced participants.
  * annotations: demographics, PHQ-9 (depression), GAD-7 (anxiety)
  * reference: ML Tlachac, Ricardo Flores, Miranda Reisch, Katie Housekeeper, Elke Rundensteiner. "DepreST-CAT: Retrospective Smartphone Call and Text Logs Collected During the COVID-19 Pandemic to Screen for Mental Illnesses." ACM IMWUT, vol. 6, no. 2, 2022.
  * ✅ available: free for academic use
  * also relevant to [Anxiety & Stress](#anxiety--stress) (GAD-7 scores)

- [StudentSADD Dataset](https://emutivo.wpi.edu/index.php/data/)
  * Student suicidal ideation and depression detection dataset.
  * annotations: suicidal ideation, depression labels
  * available: tbd (see project page)
  * also listed under [Suicide Risk & Crisis Intervention](#suicide-risk--crisis-intervention)




---

### AVEC Challenge Datasets
  
The Audio/Visual Emotion Challenge (AVEC) series released several benchmark datasets, many of which are directly relevant to depression detection. Listed separately here as they are frequently searched for by name, even though several overlap with the DAIC family above.
  
  - **AVEC 2013 / AVEC 2014** — based on the AVEC/AViD-Corpus (audio-visual depressive language corpus) (link deprecated - tbd), with self-reported BDI-II depression scores.
    * 📧 available: upon request via the challenge organizers
  
  - **AVEC 2016 / AVEC 2017** — Depression sub-challenge based on DAIC-WOZ (see above).
    * 📧 available: upon request for academics (DAIC-WOZ)
  
  - **AVEC 2018** — Turkish Audio-Visual Bipolar Disorder Corpus (see bipolar below) - no longer available
  
  - **AVEC 2019** — "Detecting Depression with AI" sub-challenge based on Extended DAIC (see above).
    * 📧 available: upon request for academics (Extended DAIC)
  
  
---

## Bipolar Disorder

- [Eye gaze and facial displays during emotional film clips in remitted BD patients](https://doi.org/10.1192/j.eurpsy.2020.26)
  * 16 patients with bipolar disorder (in remission) and 16 matched healthy controls watched 7 emotional film clips (~13 min total) while facial movements (16 AUs via OpenFace) and eye gaze were recorded.
  * annotations: BD/HC group label, HDRS-17, YMRS, demographics
  * reference: Kjærstad HL, Jørgensen CK, Broch-Due I, et al. (2020). "Eye gaze and facial displays of emotion during emotional film clips in remitted patients with bipolar disorder." Eur Psychiatr. 63(1):e29.
  * 🔒 available: not publicly available (contact authors)

- [Turkish Audio-Visual Bipolar Disorder Corpus](https://ieeexplore.ieee.org/document/8470362/)
  * Audio-visual corpus for affective computing and psychiatric research on Bipolar Disorder; was part of AVEC 2018.
  * annotations: Bipolar Disorder yes/no (binary labels)
  * reference: "The Turkish Audio-Visual Bipolar Disorder Corpus", Ciftci, Kaya (2018)
  * ❌ has become unavailable. (Permitted use ran out, listed for completeness.)

- [Depresjon](https://datasets.simula.no/depresjon/) — see [Depression](#depression); also includes bipolar patients.

---

## Schizophrenia & Psychosis

Includes datasets on diagnosed psychotic disorders as well as individuals at ultra-high risk (UHR) / clinical-high-risk (CHR) for psychosis.

- [FOCUS trial](https://pubmed.ncbi.nlm.nih.gov/25623736/) 
  * FOCUS trial (Function and Overall Cognition in Ultra-high risk States) is a randomised, parallel group, observer-blinded clinical trial enrolling 126 patients meeting the standardised criteria of being at UHR for psychosis.
  * 45-second videotaped "audition" task (High-Risk Social Challenge, HiSoC) from 108 individuals at ultra-high risk (UHR) for psychosis and 65 matched healthy controls.
  * annotations: UHR/HC group label, CAARMS (attenuated psychotic symptoms), SANS (negative symptoms), HiSoC social skills ratings (16 items + 3 factors + general impression + total), demographics (age, sex, parental SES), medication status (antipsychotic naive/exposed), DSM diagnoses, substance use
  * reference: Glenthøj LB, Fagerlund B, Randers L, Hjorthøj CR, Wenneberg C, Krakauer K, Vosgerau A, Gluud C, Medalia A, Roberts DL, Nordentoft M. "The FOCUS trial: cognitive remediation plus standard treatment versus standard treatment for patients at ultra-high risk for psychosis: study protocol for a randomised controlled trial." Trials. 2015 Jan 27;16:25. doi: 10.1186/s13063-014-0542-8. PMID: 25623736; PMCID: PMC4318160.
  * 🔒 not available: not publicly available (contact authors)


---

## Autism & Neurodevelopmental Disorders

- [A Dataset of Eye Movements for Children with Autism Spectrum Disorder](https://zenodo.org/records/2647418)
  * 300 natural scene images and corresponding eye movement data. 14 children with ASD and 14 healthy controls.
  * annotations: ASD / control labels, eye movement trajectories
  * reference: H. Duan, G. Zhai, X. Min, Z. Che, Y. Fang, X. Yang, J. Gutiérrez, P. Le Callet. "A Dataset of Eye Movements for the Children with Autism Spectrum Disorder." ACM MMSys'19, Jun. 2019.
  * ✅ available: free to download


- [CALMED (Children, Autism, Multimodal, Emotion, Detection)](https://link.springer.com/chapter/10.1007/978-3-031-35681-0_43) ([arxiv](https://arxiv.org/abs/2307.13706))
  * Audio and video features extracted from study sessions with children with ASD (level 1 diagnosis), aged 8–12. 57,012 examples, each representing a 200ms time window. Annotations provided by parents into four target emotion classes.
  * annotations: 4-class emotion labels (parent-annotated), ASD diagnosis (level 1)
  * reference: Sousa A, Young K, d'Aquin M, Zarrouk M, Holloway J. "Introducing CALMED: Multimodal Annotated Dataset for Emotion Detection in Children with Autism.", In: Universal Access in Human-Computer Interaction, HCII 2023. Lecture Notes in Computer Science, vol 14020. Springer, Cham. doi: 10.1007/978-3-031-35681-0_43
  * code: [github](https://github.com/annanda/emotion_detection_for_children_with_asd)
  * 🔒 available: does not seem to be available (check with authors)

- [Hugging Rain Man (HRM) Dataset](https://ieeexplore.ieee.org/document/10955738/) [github](https://github.com/Jonas-DL/Hugging-Rain-Man)
  * ~130,000 frames of posed and spontaneous facial expressions from 98 children
    (66 ASD, 32 TD), aged 2–12. Manually annotated by FACS experts. Raw images are
    not publicly available due to privacy/ethics; AU labels, extracted features, and
    pre-trained models are released.
  * annotations: 22 Facial Action Units (AUs), 10 Action Descriptors (ADs), atypicality ratings, ASD/TD group label (DSM-5 criteria)
  * reference: Ji Y, Wang S, Xu R, Chen J, Quan Y, Jiang X, Deng Z, Liu J., "Hugging Rain Man: A Novel Facial Action Units Dataset for Analyzing Atypical Facial Expressions in Children with Autism Spectrum Disorder." IEEE Transactions on Affective Computing. 2025; 16:2287-2302.doi: 10.1109/TAFFC.2025.3558914
  * ✅ available: AU labels, extracted features, and pre-trained models publicly available (CC BY-NC-SA 4.0, non-commercial research only)
      * not available: raw images have not been released — see [github](https://github.com/Jonas-DL/Hugging-Rain-Man)


- [DE-ENIGMA Dataset](https://cordis.europa.eu/project/id/688835)
  * Multimodal dataset of children with ASD interacting with a humanoid robot during therapy sessions, including facial mapping coordinates, visual and audio data.
    EU H2020-funded project across multiple countries/cultures aimed at enhancing social imagination skills in children with ASD.
  * annotations: engagement, affect, and behavioural labels; facial, vocal and verbal cues
  * reference: Riva G, Riva E. "DE-ENIGMA: Multimodal Human–Robot Interaction for Teaching and Expanding Social Imagination in Autistic Children." Cyberpsychology, Behavior, and Social Networking. 2020;23(11):806-807. doi: 10.1089/cyber.2020.29200.ceu
  * 🔒 not available ([project website](de-enigma.eu) no longer available)


---

## Anxiety & Stress

- [DASPS Database](https://ieee-dataport.org/open-access/dasps-database) (2021)
  * Raw EEG data collected from 23 participants during anxiety-inducing situations. Includes a MATLAB script for segmenting each EEG signal into 6 segments corresponding to 6 situations.
  * annotations: anxiety levels across 6 situations
  * ✅ available: open access (IEEE DataPort)

- [Extended DAIC Database](https://dcapswoz.ict.usc.edu/) — see [Depression](#depression); includes PCL-C (PTSD) scores alongside PHQ-8.

- [The DepreST Call and Text (DepreST-CAT) Dataset](https://github.com/mltlachac/DepreST-CAT) — details see [Depression](#depression); includes GAD-7 (anxiety) scores.


---

## Infant & Early Development


- [Infant Facial Affect (IFA) — Mother-Infant Free-Play Dataset](https://doi.org/10.1016/j.infbeh.2017.05.007)
  * 71 mother-infant dyads (4-month-olds; 24 with maternal PPD, 47 typical), recorded during a 10-minute face-to-face free-play session. Frame-by-frame IFA coding (positive/neutral/negative, 3 min per dyad).
  * annotations: IFA affect labels — 5 categories (positive high/low, neutral, negative high/low); commonly collapsed to 3 (positive/neutral/negative), maternal PPD status, EPDS scores, demographics.
  * reference: Egmose I, Cordes K, Smith-Nielsen J, Væver MS, Køppe S. "Mutual regulation between infant facial affect and maternal touch in depressed and nondepressed dyads." Infant Behavior and Development. 2018;50:274-283. doi: 10.1016/j.infbeh.2017.05.007
  * 🔒 available: not publicly available

- [The Craniofacial Microsomia: Longitudinal Outcomes in Children pre-Kindergarten (CLOCK)](https://pubmed.ncbi.nlm.nih.gov/30621445/) (2019)
  * Longitudinal cohort study of neurobehavioural outcomes in infants and toddlers with craniofacial microsomia (CFM). 108 cases and 84 controls recruited from 5 US craniofacial/otolaryngology clinics, followed from age 12–24 months to age 36–48 months. Includes phenotypic, neurodevelopmental, and facial expression assessments.
  * annotations: CFM severity (PAT-CFM), neurodevelopmental outcomes (Bayley-III, CELF-P2), hearing loss, social communication, demographics
  * reference: Luquetti DV, Speltz ML, Wallace ER, et al. "Methods and Challenges in a Cohort Study of Infants and Toddlers With Craniofacial Microsomia: The CLOCK Study." Cleft Palate Craniofac J. 2019;56(7):877-889. doi: 10.1177/1055665618821014
  * 🔒 available: not publicly available


- [MIAMI](https://pubmed.ncbi.nlm.nih.gov/26640622/) (2015)
  * Head movement dynamics of 42 4-month-old infants and their mothers during the Still Face paradigm (Play → Still Face → Reunion, 2 min each). Angular displacement and velocity measured using the CSIRO head tracker.
  * annotations: head movement dynamics (angular displacement, angular velocity), interaction phase labels (Play, Still Face, Reunion)
  * reference: Hammal Z, Cohn JF, Messinger DS. "Head Movement Dynamics During Play and Perturbed Mother-Infant Interaction." IEEE Trans Affect Comput. 2015 Oct-Dec;6(4):361-370. doi: 10.1109/TAFFC.2015.2422702
  * 🔒 available: not publicly available



---

## Suicide Risk & Crisis Intervention

- [StudentSADD Dataset](https://emutivo.wpi.edu/index.php/data/)
  * Student suicidal ideation and depression detection dataset.
  * annotations: suicidal ideation, depression labels
  * available: see project page
  * full entry also listed under [Depression](#depression)

---

## Multimodal and General Mental Health Resources

Related and beyond stuff (remove?).
General affective-computing or multi-domain resources that are not specific to a single diagnostic category but are commonly used in mental health ML pipelines.

- [MultiWOZ — A Large-Scale Multi-Domain Wizard-of-Oz Dataset for Task-Oriented Dialogue Modelling](https://aclanthology.org/D18-1547/)
  * 10k dialogues (3,406 single-domain, 7,032 multi-domain). General dialogue dataset, occasionally used as pretraining/background data for conversational mental health agents.
  * reference: Paweł Budzianowski et al. "MultiWOZ - A Large-Scale Multi-Domain Wizard-of-Oz Dataset for Task-Oriented Dialogue Modelling." EMNLP 2018, Brussels.
  * 📧 available: upon request for academics


## Related Resources (Not Mental Health Datasets)

- [YouTube Facial Palsy (YFP) Database](https://sites.google.com/view/yfp-database) (2018)
  * 32 videos of 21 patients from YouTube; some patients have multiple videos. Not a mental health dataset per se, but relevant for facial AU/expression pipelines applied across clinical populations.
  * annotations: manually labelled local palsy regions, location (eyes, mouth), intensity (low or high)
  * reference: Gee-Sern Jison Hsu, Jiunn-Horng Kang, Wen-Fong Huang. "Deep Hierarchical Network With Line Segment Learning for Quantitative Analysis of Facial Palsy." IEEE Access, vol. 7, 4833-4842, Dec. 2018.
  * 📧 available: upon request for academics

- [RAVDESS](https://zenodo.org/record/1188976) (2018)
  * The Ryerson Audio-Visual Database of Emotional Speech and Song. 7356 recordings, each rated 10 times on emotional validity, intensity, and genuineness by 247 individuals.
  * subjects: 24 professional actors (12 female, 12 male)
  * annotations: emotion + intensity — calm, happy, sad, angry, fearful, surprise, disgust at two intensity levels + neutral
  * reference: Livingstone SR, Russo FA (2018). "The Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS)." PLoS ONE 13(5).
  * ✅ available: Creative Commons Attribution


---

## Related Resources

1. **Face analysis datasets, AU tools, face models** →
   [AutomaticFaceAnalysis](https://github.com/stellagra/AutomaticFaceAnalysis)

2. **Human motion & sports** →
   [HumanMotionCollection](https://github.com/stellagra/HumanMotionCollection)

3. **More mental health datasets** →
   [emutivo.wpi.edu](https://emutivo.wpi.edu/index.php/data/)

4. **Pioneer Centre for AI: P1 program — Bridging Minds and Machines (AI, HCI & Psychology)** →
   [aicentre.dk](https://www.aicentre.dk/p1-programs/bridging-minds-and-machines-ai-hci-psychology)

---

## 2DO
- add overview table
- add missing info
- check if [EMU](https://github.com/mltlachac/EMU) or [here](https://emutivo.wpi.edu/index.php/data/) should be added (depression? audio+text)
- Check [list of databases by Mahoor](https://mohammadmahoor.com/pages/databases/) for additional entries

---

## Contact
[Stella Grasshof](https://pure.itu.dk/en/persons/stella-grasshof) - IT University of Copenhagen

<p align="right">[<a href="#readme-top">back to top</a>]</p>
