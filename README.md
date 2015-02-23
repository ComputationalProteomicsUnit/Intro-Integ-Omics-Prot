# Introduction to Integrative Omics


- http://www.ebi.ac.uk/training/course/introduction-integrative-omics
- Tuesday, March 3, 2015 - Friday, March 6, 2015
- European Bioinformatics Institute

| When              | What                                              |
|-------------------|---------------------------------------------------|
| Wed 17:30 - 18:00 |  ~~Keynote Lecture II~~ Intoduction to proteomics |
| Thu 09:00 - 10:30 | The nature of proteomics data – caveats for integration ~~(Tutorial with hands on)~~ |

## Introduction to proteomics

- Introduction to MS-based proteomics, to give participants a fair
  understanding of proteomics data, in terms of quantitation and
  identification.

- Challenges of MS-based proteomics

- What can we assays with proteomics: differential protein expression,
  post-translational modifications, protein-protein interactions,
  spatial proteomics.

## Integrating proteomics data

Similarities and, most importantly, differences with high-throughput
sequencing data.

Examples and discussion of proteomics data integration (with `R` code).



### Mapping peptides to genomic coordinates: =Pbase=, but see also others.

Different approaches to integration exist: (i) model- or network-based
approaches that identify common patterns in different data sources as
well as (ii) reference-based approaches, that map different sources of
data against a common reference. The former are very versatile and
rely on experiment-wide clustering/modelling
\cite{Le_Cao:2011,Haider:2013, Meng:2014} and crucially depend on
reliably linking features (explicitly via common identifiers or
through functional contextualisation). Transcript and protein
measurement have previously been combined and compared by linking the
respective features by a common gene identifier
\cite{Lundberg:2010,Nagaraj:2011}. Such approaches are often difficult
to track and are susceptible to inconsistencies in the relation
between different data sources when, for example, multiple transcripts
are compared to ambiguous protein groups. The latter approaches are a
natural choice for data stemming from genomics, transcriptomics,
epigenomics, etc that directly rely on mapping their data features
along a genome reference.

#### Mapping, database reduction, database expansion

- [Pang et al. (2014)](http://www.ncbi.nlm.nih.gov/pubmed/24152167)
- [Evans et al. (2012)](http://www.ncbi.nlm.nih.gov/pubmed/23142869)
- [Sheynkman et al. (2014)](http://www.ncbi.nlm.nih.gov/pubmed/25149441)
- [Wang and Zhang (2013)](http://www.ncbi.nlm.nih.gov/pubmed/24058055) [`customProDB`](http://bioconductor.org/packages/release/bioc/html/customProDB.html)



### Combining quantitative spatial proteomics and (binary) annotation features

- thetaOptimisation
