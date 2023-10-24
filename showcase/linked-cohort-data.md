---
title: Linked pathogen and host data across archives - a multi-omics, SARS-CoV-2 cohort case study
contributors: [Gabriele Rinck, Zahra Waheed] 
description: Here we describe the first example of linking and sharing a COVID-19, multi-omics cohort data set via the EMBL-EBI infrastructure. 
affiliations: [EMBL-EBI]
page_id: LinkedCohortData

# More information on how to fill in this metadata section can be found here https://www.infectious-diseases-toolkit.org/contribute/page-metadata
---

<!-- Please take in mind our style guide https://www.infectious-diseases-toolkit.org/contribute/style_guide when writing the content of this page. -->

<!--- Showcase pages should detail a particular combination of standards and tools from an infrastructural or domain perspective to tackle infectious diseases related data challenges. --->

## The importance of data integration 

Cohort studies produce invaluable data typically including a range of different data types, such as clinical (e.g. patient health records, blood markers, treatment details) as well as multi-omics data (such as genomic sequence, transcriptomic or proteomic data). However, often these data types are siloed in archives specific for each type. Data integration, i.e, linking these data types on a participant level across different repositories, adds more depth to the dataset by bringing the pathogen and host data into context, allowing a more comprehensive analysis of the entire collection of data. 
Here we describe the first example of linking and sharing a multi-omics SARS-CoV-2 cohort dataset with multiple time points, via the European Molecular Biology Laboratory-European Bioinformatics Institute’s (EMBL-EBI) infrastructure. 


## Who is the SHOWCASE intended for?

This showcase is intended for any groups who would like to FAIRly share cohort study data, and would like to better understand how this can be performed. More broadly, the linking mechanism described below is applicable to any group whose research involves different types of molecular data being obtained from the same biological sample. 
The showcase will also be useful for those wishing to access linked clinical and multi-omics data from cohort studies. 

## The process of sharing a Linked Cohort Dataset

**Image goes here** 
Figure N provides an overview of the data integration process across the EMBL-EBI archives. 

The work presented here was a coordinated effort of multiple teams at Erasmus Medical Centre (data collection and submission) and EMBL-EBI (repository infrastructure for data sharing) with the support of University Hospital Heidelberg (harmonisation of clinical-epidemiological data), part of the ReCoDID project (funded by the European Union’s Horizon 2020 Research and Innovation Programm (Grant Agreement No.825746) and the Canadian Institutes of Health Research, Institute of Genetics (CIHR-IG) (Grant Agreement N° 01886-000)). It showcases the process of how cohort datasets (or other datasets consisting of multiple data types) can be linked and shared using the EMBL-EBI infrastructure.
 


The data was collected from a cohort of 151 PCR-confirmed COVID-19 individuals who had been admitted to the EMC hospital with a respiratory infection or respiratory failure in 2020-2021. After harmonisation of the clinical-epidemiological data using the ISARIC data dictionary (carried out by ReCoDID partners at the university hospital in Heidelberg, Germany), the pseudonymised clinical-epidemiological data were submitted to the European Genome-phenome Archive (EGA), SARS-CoV-2 sequences were deposited in European Nucleotide Archive (ENA) and ArrayExpress/BioStudies was used to archive antibody profiles as well as B-cell and T-cell data (see figure N). 

The various data types were linked on participant level by utilising the BioSamples data archive which can capture relationships between samples. In a hierarchical structure a top-level sample ID was created which represents the patient (and the associated EGA record). Further BioSample IDs were created for each time point and/or data type and these were linked to the top-level sample ID of this patient, creating a link between data types on participant level.
The Composition of the EMC Pilot Dataset is shown in figure M below:

- Clin-epi information for all 151 patients that tested PCR-positive for SARS-CoV-2. For 77 of those additional data types are available and these have also been submitted and linked; for the remaining 74 patients only clin-epi data is available. (Archived in EGA, access managed through DAC);
- 80 SARS-CoV-2 sequences are available for 63 patients, with 1-4 sequences per patient. (Archived in ENA, open access);
Antibody profiles are available for 40 patients with 2-5 time points per patient, with a total of 147 data points. (Archived in ArrayExpress/BioStudies, open access);
- T-cell data are available for 28 patients with 1, 3 or 4 time points per patient and a total of 51 data points. (Archived in BioStudies, open access);
- B-cell data are available for 17 patients with either one or 3 time points and a total of 29 data points. (Archived in ArrayExpress/BioStudies, open access).


**Figure M:** A Venn diagram showing the different combinations of data types for all 151 patients.

This showcase provides a proof of concept for linking and sharing of entire cohort datasets in compliance with FAIR principles with data sharing being as open as possible and as closed as necessary. The applied linking process significantly increases the interoperability between the bespoke archives for the various data types, making it easier to access and analyse the associated data types. 



<!--- In this section you should provide a brief description of what the showcase is i.e. what it comprises of and a general description for it.  --->
<!--- Start with a graphical representation of the showcase, with a caption and an alternative text (alt). The graphical representation should be a diagram showing the different standards, tools, data sources that are used to tackle the challenge. The diagram should show how these different modules connect with one another  --->
{% include image.html file="" caption="Figure 1. " alt="" %}

Link to dataset in biosamples

## Cohort Browser

A Cohort Browser serves as the primary entry point into cohort data. It lists discovery metadata of cohort studies and provides links to the available data types. Where possible, basic aggregate data are also included. Search and filtering functionality will allow the users to locate datasets of interest. 

## What can you use the SHOWCASE for?
 <!--- In this section you should provide a brief summary of the uses of the showcase, i.e. when you would use this showcase resource --->

This showcase provides a proof of concept for linking and sharing of entire cohort datasets in compliance with FAIR principles with data sharing being as open as possible and as closed as necessary.  

- Link different biological data types, at the sample-level, across archives specific to biological data types (while cross referencing exists, this has not been done before on the sample level: https://www.nature.com/articles/s41597-019-0258-4). This is the first such study in the public domain.
- The applied linking process significantly increases the interoperability between the bespoke archives for the various data types, making it easier to access and analyse the associated data types.
- Linking these data types on a participant level also adds more depth to the dataset by bringing the pathogen/host data into context, allowing a more comprehensive analysis.
- This is particularly important in public health but will equally provide a better understanding of infectious diseases in the context of both pathogen & their host factors
