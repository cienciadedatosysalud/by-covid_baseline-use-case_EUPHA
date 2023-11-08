![logo](https://eupha.org/images/EUPHA_logo.svg)
![logo2](https://ephconference.eu/site_images/logo_EPH_site.svg)
# Pre-conference: Reuse of sensitive individual data – Methods and tools for a federated approach
---
# BY-COVID Baseline Use Case (EUPHA)
### - Author: **Francisco Estupiñan-Romero**, Institute for Health Sciences in Aragon (Spain)
### - Email: <festupinnan@iacs.es>


### - Author: **Enrique Bernal-Delgado MD PhD**, Institute for Health Sciences in Aragon (Spain)
### - Email: <ebernal@iacs.es>


---

# Translate the research question into a Common Data Model.

To do this, we are going to use the Common Data Model Builder (cdmb) library.
The Common Data Model Builder (cdmb) is a Python library that facilitates the construction of data models for projects with a defined structure.

Link to the Python library:

https://github.com/cienciadedatosysalud/cdmb

Link to the tutorial (EUPHA):

https://github.com/cienciadedatosysalud/tutorial_cdmb_EUPHA

Configuration file for by-covid_baseline-use-case_EUPHA (cdmb_config.json)

[docs/CDM/cdmb_config.json](https://github.com/cienciadedatosysalud/by-covid_baseline-use-case_EUPHA/blob/main/docs/CDM/cdmb_config.json)

It's time to start the [tutorial](https://github.com/cienciadedatosysalud/tutorial_cdmb_EUPHA)! 🦾

---

# Technical part (💻)

If you have reached this point you have successfully completed the tutorial, **congratulations!**

Let's review what you get when using the Common Data Model Builder library.

- A fixed and standardized folder structure in which to develop the analysis scripts. A structure where all the information entered by a domain expert is collected and expressed in a way that a computer scientist can easily interpret
- Project information
- Cohort information
- Information of all defined entities:
  - Syntactic and semantic information of all variables of each entity.
  - Catalogues used to define the entity.
  - Validation rules.
  - Synthetic data 
- Data Quality Assessment script
- Rule validation report script
- Header and syntax checking script for csv input files

---

# Distribution (🌎)
Once the analyses have been developed.

How is your project distributed? 

One of the alternatives is to containerize your application (e.g., Docker, Singularity). 

To learn more, visit the [ASPIRE (Analytic Software Pipeline Interface for Reproducible Execution)](https://github.com/cienciadedatosysalud/aspire) repository. 

(APIRE has been used for the distribution of this Use Case.)

## HOW TO RUN IN DOCKER
Use the following code snippet to create the container.
```bash
docker pull ghcr.io/cienciadedatosysalud/bycovid-eupha:latest

docker run -d -p 127.0.0.1:3000:3000 --name bycovid-eupha-aspire ghcr.io/cienciadedatosysalud/bycovid-eupha:latest

# Open your web browser at http://localhost:3000.
```

## HOW TO RUN IN SINGULARITY
Use the following code snippet to create the container.
```bash
singularity build bycovid-eupha.sif docker://ghcr.io/cienciadedatosysalud/bycovid-eupha:latest

singularity run -f -w bycovid-eupha.sif

# Open your web browser at http://localhost:3000.
```

# References
- Common Data Model Builder Tutorial (Google Colab): https://github.com/cienciadedatosysalud/tutorial_cdmb_EUPHA
- BY-COVID - WP5 - Baseline Use Case: SARS-CoV-2 vaccine effectiveness assessment: https://github.com/by-covid/BY-COVID_WP5_T5.2_baseline-use-case
- Data Science for Health Services and Policy Research group: https://cienciadedatosysalud.org/en/
- Common Data Model Builder library: https://github.com/cienciadedatosysalud/cdmb
- Analytic Software Pipeline Interface for Reproducible Execution (ASPIRE): https://github.com/cienciadedatosysalud/ASPIRE
- Atlas VPM community in Zenodo: https://zenodo.org/communities/atlasvpm
- Research Object Crate (RO-Crate): https://www.researchobject.org/ro-crate/
- ORCID: https://orcid.org/

<a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" ><img src="https://img.shields.io/badge/license-CC--BY%204.0-lightgrey" alt="License: CC-BY 4.0"></a>

