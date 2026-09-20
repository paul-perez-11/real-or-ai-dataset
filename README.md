# Real or AI Dataset
## Overview
This repository contains the primary and derived datasets from a behavioral survey evaluating the audio deepfake detection capabilities of 173 undergraduate students at Mapúa University. The data was collected as part of an unpublished freshman research paper titled *"REAL OR AI?: A QUANTITATIVE STUDY ON THE DEEPFAKE DETECTION ABILITY OF UNDERGRADUATE STUDENTS AT MAPÚA UNIVERSITY"*.

## Dataset Description
The study required participants to listen to 10 sequential audio clips—a mix of real and AI-generated speech—one at a time. For each clip, respondents provided a binary classification (Real vs. AI) and assigned a subjective confidence score on a sliding scale from 1 to 100.

The repository includes the following primary files:
* **Real or AI Dataset (ANONYMIZED).csv:** The raw survey responses containing 173 rows and 26 columns. It tracks demographic information (Program, Year, School), the chronological presentation sequence of the clips ("View Order"), and an experimental grouping variable (Control vs. Experimental). The Experimental group received a short training video prior to testing.
* **Real or AI Dataset (SDT ANALYSIS).csv:** A supplementary dataset containing mathematically derived psychological metrics using Signal Detection Theory (SDT). It separates each respondent's actual detection ability (sensitivity, or $d'$) from their psychological tendency to guess (response bias, or $\beta$).
* **Master Key:** The ground-truth answer key detailing which of the 10 clips were bona fide human audio and which were AI deepfakes.

## Data Dictionary (Key Variables)
* `Participant`: Anonymized integer identifier.
* `Group`: Indicates whether the student was in the Control group or Experimental group.
* `View Order`: A parsed string detailing the exact chronological sequence of the 10 clips presented to the respondent.
* `Q[Odd Numbers]`: The categorical classification decision (Real or AI) for the clip.
* `Q[Even Numbers]`: The self-reported confidence score (1-100) for the preceding decision.

## Disclaimer
This dataset was collected in late 2025 by freshman undergraduate students. The associated research paper has not yet been formally published or peer-reviewed. All respondent data has been fully anonymized.
