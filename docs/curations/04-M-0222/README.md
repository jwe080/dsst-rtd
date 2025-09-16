# NIMH Ketamine Mechanism of Action Study

The study was completed at the National Institute of Mental Health (NIMH) Intramural Research Program (IRP)  (ID: 04-M-0222) within the within the Experimental Therapeutics and Pathophysiology Branch.  It is a double-blind placebo cross-over trial of a single infusion of ketamine or saline placebo which included both patients and healthy volunteers. Patients with major depressive disorder (MDD) were medication-free for at least 2 weeks prior to the start of the study. Recruitment for the bipolar (BP) group was ended early on, but is included here for completeness. Some measurements (tasks/scans/scales) were added part-way into the study and have fewer completed measurements.

Nominally, there are five Magnetic Resonance Imaging (MRI) scans per subject at both 3 Tesla with the details listed below. Note that not all planned scans were completed: some participants dropped out of the trial, some people did not want to have an MRI (infrequent), and sometimes there were technical issues.

## MRI Data Description

Scans are normally performed at baseline (b0) (about 2 days before) and then 2-3 (d2/p2) and 10-11 (d10/p10) days after blinded infusion on a 3T GE Signa HDx with an 8 channel head coil unless otherwise specified.

- Subjects: total N = 58
  - n, Group 1 (MDD) = 33
  - n, Group 2 (BP) = 3
  - n, Group 3 (HC) = 22
- Sessions per subject: total = 5
  - Baseline (b0)
  - Post-infusion 1 (ketamine: d2 or placebo: p2)
  - Interim 1 (ketamine: d10, or placebo: p10)
  - Post-infusion 2 (opposite, ketamine: d2 or placebo: p2)
  - Interim 2 (ketamine: d10, or placebo: p10)
- Session identifiers are documented in the `phenotype/phenotype.json` file
- Anatomical runs per session:
  - T1-weighted: 1 run (often 1 or 2 additional T1-weighted runs in the baseline session)
  - T2-weighted: 3 runs (baseline session only)
- Diffusion-Weighted Imaging (DWI): 2 runs (baseline session only)
  - 30 directions, bval: 1100 s/mm^2, acquired in two groups (g1/g2)

- Functional runs per session:
  - Resting state: 1 run, 8 min, eyes closed, physio was collected during this run only (for most of the data)
  - [Dot probe task](https://www.sciencedirect.com/science/article/pii/S2213158218302183): 2 runs, 8.75 min each. This task used a mixed block/event-related design. In each trial, a fixation cross was presented for 500 ms in the center of the screen, where the participant had been instructed to focus. This was followed by two faces presented side by side for 500 ms; one displayed an angry, happy, or neutral expression and the other was always neutral. After the faces were presented, a single dot was presented on one side for 200 ms, to which the participant responded with a button press to indicate whether the dot probe was on the left or right. Trials in which the dot replaced the emotional face were considered congruent, according to the expectation of attention being biased more towards an emotional than a neutral face. Trials in which the dot replaced the neutral face were considered incongruent. Trials were randomized and counterbalanced for emotion, gender of face, side of emotional face, and side of probe. There was then an interstimulus interval in which a blank screen appeared for 1300 ms. Jitter was randomly added in as additional trials in which only a fixation cross appeared in place of the faces and probe. Trials were grouped into blocks: angry blocks comprised trials with angry and neutral faces or two neutral faces, and happy blocks comprised trials with happy and neutral faces or two neutral faces. The task comprised two runs, and each run included one angry block and one happy block. For each scanning session, the task used a unique set of facial stimuli that were counterbalanced between the ketamine and placebo arms of the study according to the randomized crossover study design.
  - [Emotional faces evaluation task](https://www.sciencedirect.com/science/article/pii/S0165032720328512): 2 runs, 4.8 min each. This task used a mixed block/event-related design. In each trial (Fig. 2), a fixation cross was presented for 500 ms in the center of the screen, where the participant had been instructed to focus. This was followed by two faces presented side by side for 500 ms; one displayed an angry, happy, or neutral expression and the other was always neutral. After the faces were presented, a single dot was presented on one side for 200 ms, to which the participant responded with a button press to indicate whether the dot probe was on the left or right. Trials in which the dot replaced the emotional face were considered congruent, according to the expectation of attention being biased more towards an emotional than a neutral face. Trials in which the dot replaced the neutral face were considered incongruent. Trials were randomized and counterbalanced for emotion, gender of face, side of emotional face, and side of probe. There was then an interstimulus interval in which a blank screen appeared for 1300 ms. Jitter was randomly added in as additional trials in which only a fixation cross appeared in place of the faces and probe. Trials were grouped into blocks: angry blocks comprised trials with angry and neutral faces or two neutral faces, and happy blocks comprised trials with happy and neutral faces or two neutral faces. The task comprised two runs, and each run included one angry block and one happy block. For each scanning session, the task used a unique set of facial stimuli that were counterbalanced between the ketamine and placebo arms of the study according to the randomized crossover study design.
  - [N-back task](https://zenodo.org/records/7148): 1 run, 6 minutes. Following an initial fixation
cross (which lasted 0.9s in duration) and block condition instructions (1s; “1-back”
or “3-back”; Figure 5.2A; these remained onscreen for the rest of the block),
participants were presented with a randomized sequence of 12 lower case consonants
(1s; “t”, “f”, “p”, “v”, “g” or “h”), between a blank screen (0.5s), save for the task
instruction; alternatively, a fixation cross was presented continuously and
participants were instructed to rest. The aim was for participants to make a button
press when the stimulus on screen was the same as the stimulus n-back. Participants
were only presented with 1- and 3-back active blocks and rest. Blocks, of which there were 18,
were randomized in order, with six of each condition presented (rest, 1-back and 3-
back). Each block lasted 19.1 seconds from the time of the instructions to the interim
fixation cross, with the task lasting six minutes in total. Only one run was undertaken
during each scanning session. Participants received extensive training on the n-back
task, completing 0-, 1-, 2-, and, 3-back examples, prior to performing the task inside
the MRI scanner

- Magnetic Resonance Spectroscopy (MRS)
  - nominally all sessions for participants after sub-MOA115/sub-MOA306
  - 7T Siemens, 32ch head coil
  - 2cm isotropic voxel centered on the perigenual ACC, [TE-optimized J-suppression PRESS sequence at 7T optimized to measure glutamate](https://pubmed.ncbi.nlm.nih.gov/24585452/)

### Exceptions

1. The anatomical data of `sub-MOA133/ses-b0` came from an excluded scan two weeks earlier in order to have anatomical data to go along with the functional data.
1. Not every functional run has an events file of timings of stimuli presented during the run.

## Tabular Phenotypic Data Description

The Montgomery-Asberg Depression Rating Scale (MADRS), the abbreviated Hamilton Rating Scale for Depression (HAMD-6), and the Hamilton Depression Rating Scale (HAMD-17) surveys participants filled out at the MRI sessions are collected in the `phenotype/` folder with the data dictionary in the `phenotype.json` file and the data itself in the `phenotype.tsv` file.

## Inclusion/Exclusion Criteria

Please see https://clinicaltrials.gov/study/NCT00088699 for a detailed list, also included below.

### INCLUSION CRITERIA

#### General patient inclusion criteria

- Male or female subjects, 18 to 65 years of age.
- Each subject must have a level of understanding sufficient to agree to all required tests and examinations and sign an informed consent document.
- Subjects must fulfill DSM-IV criteria for Major Depressive Disorder (MDD) without psychotic features, based on clinical assessment and confirmed by a structured diagnostic interview, SCID-P.
- Subjects must have an initial score of at least 20 on the MADRS at screen and at baseline of study phase I.
- Subjects must have failed to respond in the past to an adequate dose and duration of at least one antidepressant (SSRI, bupropion, or venlafaxine) during a depressive episode
- Current depressive episode of at least 4 weeks duration.
- Additional inclusion criteria for substudy 4 (patients with MDD):
  - Age of onset less than 40 years of age.
  - Subjects with MDD must fulfill DSM-IV criteria for Major Depression single episode or recurrent without psychotic features based on clinical assessment and confirmed by a structured diagnostic interview (SCID-P).
  - A failed adequate trial of ECT would count as an adequate antidepressant trial.
  - In women of childbearing age, a negative pregnancy test within 24 hours of MRI.
- Inclusion criteria for healthy control subjects (Substudy 4 only)
  - Age 18-65 years.
  - Written informed consent completed.

### EXCLUSION CRITERIA

#### General patient exclusion criteria

- Current or past diagnosis of Schizophrenia or any other psychotic disorder as defined in the DSM-IV.
- Subjects with a history of DSM-IV drug or alcohol dependency or abuse (except for nicotine or caffeine) within the preceding 3 months.
- Female subjects who are either pregnant or nursing.
- Serious, unstable illnesses including hepatic, renal, gastroenterologic, respiratory, cardiovascular (including ischemic heart disease), endocrinologic, neurologic, immunologic, or hematologic disease.
- Subjects with uncorrected hypothyroidism or hyperthyroidism.
- Subjects with one or more seizures without a clear and resolved etiology.
- Treatment with a reversible MAOI within 4 weeks prior to study phase I.
- Treatment with fluoxetine within 5 weeks prior to study phase I.
- Treatment with any other concomitant medication not allowed (Appendix A for Substudy 2; Appendix G for Substudy 4) 14 days prior to study phase I.
- No structured psychotherapy will be permitted during the study.
- Current NIMH employee/staff or their immediate family member.
- Additional Exclusion Criteria for substudy 2 (patients with MDD)
  - Previous treatment with ketamine or hypersensitivity to amantadine.
- Additional Exclusion Criteria for Substudy 4 (patients with MDD)
  - Subjects who currently are using drugs (except for caffeine or nicotine), must not have used illicit substances in the 2 weeks prior to screen and must have a negative alcohol and drug urine test (except for prescribed benzodiazepines) urine test at screening.
  - Presence of any medical illness likely to alter brain morphology and/or physiology (e.g., hypertension, diabetes) even if controlled by medications.
  - Clinically significant abnormal laboratory tests.
  - For imaging procedures, Presence of metallic (ferromagnetic) implants (e.g, heart pacemaker, aneurysm clip).
  - Subjects who, in the investigator's judgment, pose a current serious suicidal or homicidal risk, or who have a MADRS item 10 score of greater than 4.
- Exclusion Criteria for healthy control subjects (Substudy 4 only)
  - Current or past Axis I diagnosis
  - Presence of metallic (ferromagnetic) implants (e.g., heart pacemaker, aneurysm clips).
  - Presence of medical illness likely to alter brain morphology and/or physiology (e.g., hypertension, diabetes) even if controlled by medications.
  - Treatment with any of the exclusionary medications detailed in Appendix G 14 days prior to Phase 1 of the Substudy 4.
  - Current or past alcohol or substance abuse or dependence diagnosis (except for nicotine or caffeine).
  - Presence of psychiatric disorders in first-degree relatives.
  - Female subjects who are either pregnant or nursing.
  - Current NIMH employee/staff or their immediate family member.
