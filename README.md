# by-covid_baseline-use-case_EUPHA


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
- Data Science for Health Services and Policy Research group: https://cienciadedatosysalud.org/en/
- Common Data Model Builder library: https://github.com/cienciadedatosysalud/cdmb
- Analytic Software Pipeline Interface for Reproducible Execution (ASPIRE): https://github.com/cienciadedatosysalud/ASPIRE
- Atlas VPM community in Zenodo: https://zenodo.org/communities/atlasvpm
- Research Object Crate (RO-Crate): https://www.researchobject.org/ro-crate/
- ORCID: https://orcid.org/

<a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" ><img src="https://img.shields.io/badge/license-CC--BY%204.0-lightgrey" alt="License: CC-BY 4.0"></a>

