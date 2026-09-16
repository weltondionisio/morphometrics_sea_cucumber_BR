## Input data structure

The raw dataset used in this study is not included in this repository because it contains unpublished data that may be used in ongoing and future studies.

The analytical notebook expects an Excel file named `morphometrics.xlsx`, organized with one row per specimen and the following 32 columns:

### Sampling and specimen information

`Sample`, `tombo`, `local`, `species`, `period`, `size`

where `Sample` identifies the sampling unit, `tombo` identifies the specimen, `local` represents the sampling locality, and `period` indicates the sampling season.

### Ossicle morphometric variables

`dorsal_button`, `ventral_button`, `feet_button`, `dorsal_tables`, `ventral_tables`, `feet_tables`, `dorsal__plate`, `ventral_plate`, `feet_plate`, `entacle_plate`, `dorsal_rods`, `ventral_rods`, `feet_rods`, `tentacle_rods`, `rosette`, `endplate`, `dorsal_basket`, `ventral_basket`, `dorsal_wheel`, `ventral_wheel`

### Environmental variables

`ph`, `temperature`, `oxygen`, `ec`, `salinity`, `ppt`

Environmental measurements are associated with sampling units (`Sample`) and may therefore be shared by multiple specimens collected within the same sampling event.

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

## Citation

This repository contains the analytical workflow associated with the manuscript listed above, prepared for submission to *Zoology*.

The complete bibliographic citation and DOI will be added upon publication.

Researchers wishing to reproduce or adapt the workflow can construct a dataset following this column structure and execute `morfo_model.ipynb` sequentially.
