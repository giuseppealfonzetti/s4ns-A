# Datasets

| File | Description | Source / licence |
|---|---|---|
| `ahi-cesd.csv`, `participant-info.csv`, `ahi-cesd-codebook.pdf` | Happiness (AHI) and depression (CES-D) scores of 295 adults randomised to 4 web-based positive-psychology interventions, measured on up to 6 occasions | Woodworth et al. (2018), *Journal of Open Psychology Data*, <https://doi.org/10.5334/jopd.35> (CC BY 4.0) |
| `parkinsons_updrs.csv` | Parkinson's telemonitoring: voice measures and UPDRS scores of 42 patients over 6 months (original column names kept on purpose; session 7 renames the few it uses to plain names at import) | Tsanas & Little, UCI ML Repository, <https://doi.org/10.24432/C5ZS3N> (CC BY 4.0) |
| `sleepstudy.csv` | Average reaction time (ms) per day for 18 subjects under sleep deprivation | Belenky et al. (2003), exported from the `lme4` R package |
| `rt_alzheimer.csv` | Simulated response times, Alzheimer patients vs controls, 10 trials per subject | Simulated for the course |
| `HappinessAlcoholConsumption.csv` | Happiness score and alcohol consumption per country | Kaggle, <https://www.kaggle.com/datasets/marcospessotto/happiness-and-alcohol-consumption>. Used in previous editions |

Built-in R datasets used in the course: `sleep` (Student, 1908) and `penguins` (R 4.5 or later).

`trial.rds` is **derived** from the two AHI-CESD csv files: 4 columns from the scores (`id`, `occasion`, `happiness = ahiTotal`, `depression = cesdTotal`), duplicates removed with `distinct(id, occasion)`, joined by `id` with the participant information, whose codes are turned into labelled factors. Students download it ready to use from session 3 on.
