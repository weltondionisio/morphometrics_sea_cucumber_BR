# Morphometrics of Brazilian Sea Cucumbers

This repository contains the analytical workflow associated with a scientific study on morphometric variation in Brazilian sea cucumbers, prepared for submission to *Zoology*.

The study investigates variation in calcareous ossicle morphology across species and coastal environments using multivariate and hierarchical Bayesian approaches.

## Study system

The analyses include six sea cucumber species sampled across four coastal localities in northeastern Brazil:

- *Chiridota rotifera*
- *Holothuria grisea*
- *Parathyone brasiliensis*
- *Pentamera paraibanensis*
- *Stolus cognatus*
- *Thyonidium seguroensis*

Sampling was conducted at Formosa, Genipabu, Pirambúzios, and Tambaba during dry and rainy periods, with multiple sampling units within localities.

## Repository contents

`morfo_model.ipynb` contains the analytical workflow used in the study, including:

- morphometric data preprocessing;
- principal component analysis (PCA);
- partial PERMANOVA and PERMDISP;
- analyses accounting for species identity and sampling structure;
- environmental correlation and multicollinearity assessment;
- hierarchical Bayesian modelling;
- MCMC diagnostics and posterior predictive checks;
- generation of figures used in the manuscript.

The notebook is intended to document the analytical procedures used in the associated study and facilitate their inspection and reproducibility.

## Input data structure

The raw dataset used in this study is not included in this repository because it contains unpublished data that may be used in ongoing and future studies.

The analytical notebook expects an Excel file named `morphometrics.xlsx`, organized with one row per specimen and the following 32 columns.

### Sampling and specimen information

`Sample`, `tombo`, `local`, `species`, `period`, `size`

where `Sample` identifies the sampling unit, `tombo` identifies the specimen, `local` represents the sampling locality, and `period` indicates the sampling season.

### Ossicle morphometric variables

`dorsal_button`, `ventral_button`, `feet_button`, `dorsal_tables`, `ventral_tables`, `feet_tables`, `dorsal__plate`, `ventral_plate`, `feet_plate`, `entacle_plate`, `dorsal_rods`, `ventral_rods`, `feet_rods`, `tentacle_rods`, `rosette`, `endplate`, `dorsal_basket`, `ventral_basket`, `dorsal_wheel`, `ventral_wheel`

### Environmental variables

`ph`, `temperature`, `oxygen`, `ec`, `salinity`, `ppt`

Environmental measurements are associated with sampling units (`Sample`) and may therefore be shared by multiple specimens collected within the same sampling event.

Researchers wishing to reproduce or adapt the workflow can construct a dataset following this column structure and execute `morfo_model.ipynb` sequentially.

## Reproducibility

The analyses were conducted in Python using packages including:

- NumPy
- pandas
- SciPy
- scikit-learn
- scikit-bio
- statsmodels
- PyMC
- ArviZ
- Matplotlib
- seaborn
- openpyxl

Random seeds are specified in the relevant analyses where applicable to facilitate computational reproducibility.

## Data availability

The analytical code is available in this repository.

The underlying morphometric and environmental dataset is not publicly available at this stage because it contains unpublished data intended for ongoing and future studies. The structure required to reproduce or adapt the analytical workflow is described above.

## Associated manuscript

**BEYOND THE SURFACE: BAYESIAN MODELLING OF HOW COASTAL ENVIRONMENTS MODULATE CALCAREOUS STRUCTURES IN MARINE ORGANISMS (ECHINODERMATA: HOLOTHUROIDEA)**

### Authors

**Victória Stevenson¹˒², Welton Dionisio-da-Silva⁴, Jéssica Prata¹˒³, Fúlvio Aurélio de Morais Freire²**

### Affiliations

¹ Laboratório de Invertebrados Paulo Young, Departamento de Sistemática e Ecologia, Universidade Federal da Paraíba, Campus I, CEP 58051-900, João Pessoa, Paraíba, Brazil.

² Programa de Pós-Graduação em Sistemática e Evolução, Departamento de Botânica e Zoologia, Universidade Federal do Rio Grande do Norte, Campus Lagoa Nova, CEP 59078-970, Natal, Rio Grande do Norte, Brazil.

³ Departamento de Sistemática e Ecologia, Universidade Federal da Paraíba, Campus I, CEP 58051-900, João Pessoa, Paraíba, Brazil.

⁴ Laboratório de Ecologia Sensorial e Comportamento de Aracnídeos (LESCA), Escola de Artes, Ciências e Humanidades (EACH), Universidade de São Paulo (USP), CEP 03828-000, São Paulo, Brazil.

### Data analysis

The statistical and computational analyses available in this repository were conducted by **Dr. Welton Dionisio-da-Silva**.

### Corresponding author

**Dr. Victória Stevenson**  
Email: [victorianuunees@gmail.com](mailto:victorianuunees@gmail.com)

## Citation and code reuse

This repository contains original analytical code developed for the associated scientific study.

If any part of the code, analytical workflow, statistical implementation, or derivative adaptation from this repository is used in a scientific publication, thesis, dissertation, report, presentation, software project, or other scholarly output, please provide appropriate attribution by citing this repository and, once available, the associated peer-reviewed article.

Until the article receives its final bibliographic reference and DOI, the repository may be cited as:

> Dionisio-da-Silva, W. (2026). *morphometrics_sea_cucumber_BR: Analytical workflow for morphometric and Bayesian analyses of Brazilian sea cucumbers* [Computer software]. GitHub. https://github.com/weltondionisio/morphometrics_sea_cucumber_BR

Repository:

https://github.com/weltondionisio/morphometrics_sea_cucumber_BR

Once the associated article is published, users of this code should also cite the final publication.

The complete bibliographic reference and DOI of the manuscript will be added to this repository upon publication.
