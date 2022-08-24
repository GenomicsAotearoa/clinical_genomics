# Genomics Aotearoa clinical genomics

---

"Stuff" relating to the [Genomics Aotearoa clinical genomics](https://www.genomics-aotearoa.org.nz/our-work/completed-projects/clinical-genomics) project. This repository is primarily from a bioinformatics perspective given I work in the bioinformatics component of this project. Much of the content included in this repository is simply a collection of notes, ideas, problems, challenges, solutions which may benefit others. It's probably going to be a work in progress and should not be taken as a final say in anything. Contribute your own notes, vent the brick walls you face, explain what you're doing in a clinical genomics, contribute your own notes, ask questions in the [discussions](https://github.com/GenomicsAotearoa/clinical_genomics/discussions) section, open an issue in the [issues](https://github.com/GenomicsAotearoa/clinical_genomics/issues) section, give your perspective on why this is all wrong and what you'd do instead or simply create a pull request to fix my grammer (come on, someone needs to catch this one!). A good starting point is to tell us who you are in the [who am I?](who_am_i.md) document. Let's collaborate :)

---

## Stuff

### Analysis/bioinformatics

Our current general workflow:

- Transfer raw whole genome sequence (WGS) data within New Zealand via [globus](https://www.globus.org/)
- Analyse data using pipelines we've created in house. These are designed to follow the [GATK best practice germline short variant discovery (SNPs + Indels)](https://gatk.broadinstitute.org/hc/en-us/articles/360035535932-Germline-short-variant-discovery-SNPs-Indels-) and prepare the data for [scout](https://clinical-genomics.github.io/scout/)
  - [human_genomics_pipeline](https://github.com/ESR-NZ/human_genomics_pipeline)
  - [vcf_annotation_pipeline](https://github.com/ESR-NZ/vcf_annotation_pipeline)
- Load vcf file and accessory files into [scout](https://clinical-genomics.github.io/scout/). This software serves as a user interface for people from the genetics laboratory to curate variants and diagnose rare genetic diseases
- Utilise a private github page to support the wellington genetics laboratory folk. This has some general information they might find useful for using scout, where they can log issues they encounter when using scout, ask questions about how the data has been analysed or hear announcements on changes I've made to the scout instance they're using (for example if I update the version of scout or load some more data)
- Store data on internal servers, the data can't go on the cloud, since currently this would mean the data goes overseas which violates data sovereignty of this data

### Brain dump notes

- [My notes on using scout as admin](https://github.com/leahkemp/scout_admin_notes)
