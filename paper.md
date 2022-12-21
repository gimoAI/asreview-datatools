---
title: 'ASReview Datatools: A Python package for managing reference files'
tags:
  - Python
  - Reference
  - Bibliography
  - Deduplication
  - Management
authors:
  - name:
    orcid:
    equal-contrib: true/false
    affiliation: "1, 2" # (Multiple affiliations must be quoted)
  - name: Author Without ORCID
    equal-contrib: true # (This is how you can denote equal contributions between multiple authors)
    affiliation: 2
  - name: Author with no affiliation
    corresponding: true # (This is how to denote the corresponding author)
    affiliation: 3
affiliations:
 - name:
   index: 1
 - name: Institution Name, Country
   index: 2
 - name: Independent Researcher, Country
   index: 3
date: 7 December 2022
bibliography: paper.bib
---

# Summary
Systematic literature reviews are a critical part of the research process, as they provide a comprehensive and objective overview of the existing evidence on a particular topic.
These reviews often involve screening large reference datasets, which can be time-consuming and error-prone.
To help researchers manage these datasets, ASReview Datatools was developed.
ASReview Datatools is a python package that provides a suite of tools for managing systematic literature review datasets.
It can be used to stack, convert and deduplicate datasets.
With the introduction of machine learning assisted screening tools such as ASReview, it is also necessary to manage labels in reference datasets.
Therefore, ASReview Datatools also offers tools that are specifically designed for managing labeled reference datasets, which can be useful during the screening phase of a systematic literature review.
To this purpose, it can also be used to create a single (labeled, partly labeled, or unlabeled) dataset from multiple datasets, and to derive a description on the content and labels of a dataset.
ASReview Datatools can be easily installed and used through PyPI.

# Statement of need
Systematic literature reviews involve a comprehensive and transparent search for relevant literature, and an evaluation of the relevance of the identified studies.
Reference management software can be a valuable resource in supporting the systematic literature review process, particularly in the organization and management of references.
Generally, researchers make use of software packages like EndNote, Mendeley and Zotero.
One key feature of these reference management software packages is the ability to import and organize references from a variety of sources.
This can be particularly useful in systematic literature reviews, where large numbers of references may be identified through the search process.
It can help researchers to more efficiently and effectively manage the large number of references.

However, most reference managers are not specifically designed to process reference datasets that include labelling decisions.
As the use of machine learning-assisted screening tools increases, there will be a growing need to manage and/or combine multiple labeled (as well as unlabeled) datasets.

In addition, every modification to a dataset may affect the outcome and should therefore be carefully documented to improve reproducibility.
Many commonly used reference management software packages are complex and opaque, making it difficult to understand the exact operations performed due to the complexity of their documentation.

ASReview Datatools has been developed to meet several requirements:
- It should be simple to use for users with minimal Python coding experience.
To this purpose, tutorials are available to facilitate users.
- Documentation should be clear, complete and concise.
- It allows for easy modification and extension development.
ASReview Datatools is open to community contributions and designed to make it easy for any user with limited coding experience to develop and customize their own extensions.

Existing software packages lack support for operations on labeling decisions.
ASReview Datatools allows combining datasets while retaining control over labeling decisions.

# Overview
ASReview Datatools can process files from any reference manager that supports the RIS export file format, as well as tabular files that use a set of predetermined column names.

ASReview Datatools provides options for five operations:
1. Describe: describes the content and labels of a dataset to help users understand the characteristics within data.
2. Convert: convert RIS file format to tabular file formats (such as CSV and Excel) or vice versa, allowing researchers to work with the data in the format that is most convenient for them.
3. Deduplicate: remove duplicates based on persistent identifiers and title/abstract.
4. Vertical stacking: combine multiple datasets into a single file, making it easier to analyze and manage the data.
5. Compose: datasets containing records with different labels (or no labels) can be assembled into a single dataset while retaining control over keeping and/or assigning labels.


# Citations


# Figures


# Acknowledgements


# References

@article{vandeSChoot:2021,
  title={An open source machine learning framework for efficient and transparent systematic reviews},
  author={van de Schoot, Rens and de Bruin, Jonathan and Schram, Raoul and Zahedi, Parisa and de Boer, Jan and Weijdema, Felix and Kramer, Bianca and Huijts, Martijn and Hoogerwerf, Maarten and Ferdinands, Gerbrich and others},
  journal={Nature Machine Intelligence},
  volume={3},
  number={2},
  pages={125--133},
  year={2021},
  publisher={Nature Publishing Group},
  doi={10.1038/s42256-020-00287-7}
}