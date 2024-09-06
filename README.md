# The Mutation Functional Annotation Contextual Data Specification

  - [About](#about)
  - [What are ontologies and how do they improve data quality?](#what-are-ontologies-and-how-do-they-improve-data-quality)
  - [The  Contextual Data Specification Package](#the--contextual-data-specification-package)
    - [Version Control](#version-control)
    - [Package Contents](#package-contents)
      - [Data Collection Template](#data-collection-template)
      - [Field and Term Reference Guides](#field-and-term-reference-guides)
      - [Curation SOP](#curation-sop)
      - [DataHarmonizer Instructions and SOP](#dataharmonizer-instructions-and-sop)
      - [New Term Request (NTR) SOP](#new-term-request-ntr-sop)
  - [Contacts](#contacts)
  - [License](#license)
  - [Acknowledgements](#acknowledgements)

## About

The Mutation Functional Annotation Data Specification captures information about viral mutations and their correlated functional impacts as described in the literature. This spec is based on the data in [Pokay](https://github.com/nodrogluap/pokay/tree/master), a manually curated repository of SARS-CoV-2 and MPOX mutation impacts. This specification will allow researchers to validate their own mutation functional annotation data format in order to overlay their own data on the [Virus-MVP](https://virusmvp.org/) heatmap, and also provide a way for curators to easily contribute new functional annotations to Pokay.

<Blurb>
<SETUP: you'll need to manual create "term request" and "field request" labels in order for the issue forms to apply them when generated. You'll also want to go through documentation and replace all the <INSERT values with appropriate information.>

## What are ontologies and how do they improve data quality for functional annotation of mutations?

Labs collect, encode and store information in different ways. They use different fields, terms and formats, they categorize variables in different ways, and the meanings of words change depending on the focus of the organization (think of the word “plant”. To someone in agriculture, “plant” could mean an organism that carries out photosynthesis, while a food regulator might understand the word “plant” to mean a factory where food products are made). This variability makes comparing, integrating and analyzing data generated by different organizations like trying to compare apples, oranges and bananas, which is difficult to do.

Ontologies are collections of controlled vocabulary that are arranged in a hierarchy, where all the terms are linked using logical relationships. Ontologies are open source and meant to represent “universal truth” as much as possible (so not tied to one organization’s vocabulary of use case). Ontologies encode synonyms, which enables mapping between the specific languages used by different organizations, and every term in the ontology is assigned a globally unique and persistent identifier. Using ontology terms to standardize functional annotation contextual data not only helps make data more interoperable by using a common language, it also helps to make contextual data [FAIR](https://www.go-fair.org/fair-principles/) (Findable, Accessible, Interoperable, Reusable).

## The Mutation Functional Annotation Contextual Data Specification Package

This specification will be implemented via a DataHarmonizer validation template, accompanying **Field** and **Term reference guides** (which provide definitions and additional specific guidance) and a curation **Standard Operating Procedure (SOP)**. New terms and/or term changes can be requested using issue request forms, with additional guidance on how to do so outline in the New Term Request (NTR) SOP. This resources are available in the files of this repository and listed below under **Package Contents**.

### Version Control

Please note that development of the specification is dynamic and it will be updated periodically to address user needs. Versioning is done in the format of `x.y.z`.

`x` = Field level changes <br>
`y` = Term value / ID level changes <br>
`z` = Definition, guidance, example, formatting, or other uncategorized changes

Descriptions of changes are provided in [release notes](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/releases) for every new version.

### Package Contents

#### Data Collection Template - TBA
- [Pathogen Genomics Package (**<INSERT SPEC TEMPLATE NAME>**)](https://github.com/cidgoh/pathogen-genomics-package/releases)
  - Template schema files can be found as `.yaml`/`.json`/`.tsv` under [pathogen-genomics-package/templates/](https://github.com/cidgoh/pathogen-genomics-package/tree/main/templates)**<INSERT SPEC TEMPLATE FOLDER NAME>**
- [DataHarmonizer App](https://github.com/cidgoh/DataHarmonizer)
  - The DataHarmonizer is a standardized browser-based spreadsheet editor and validator.
  - Instructions on "Getting Started" downloading and using the application can be found under **DataHarmonizer Instructions and SOP** below.
  - Further information about application functionality can be found on the [DataHarmonizer Wiki](https://github.com/cidgoh/pathogen-genomics-package/wiki/DataHarmonizer-Getting-Started).

#### Field and Term Reference Guides
- [XLSX version](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/blob/main/Reference%20Guide/FunctionalAnnotation_Master-Reference-Guide_v0.0.0.xlsx)
- PDF version
  - [Field Reference Guide](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/blob/main/Reference%20Guide/FunctionalAnnotation_Master-Reference_Field-Reference-Guide_v0.0.0.pdf)
  - [Term Reference Guide](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/blob/main/Reference%20Guide/FunctionalAnnotation_Master-Reference_Term-Reference-Guide_v0.0.0.pdf)
- [Online version](https://docs.google.com/spreadsheets/d/16RBFfz-GTK6cN5rxQA-Z9H-OKEcRqTkOWuJb5AOz1Eg/edit?usp=sharing)

#### Curation SOP - TBA
- [PDF version]()
- [Online version]()

#### DataHarmonizer Instructions and SOP - TBA
- [PDF version]()
- [Online version]()

#### New Term Request (NTR) SOP - TBA
- [PDF version]()
- [Online version]()

## Ontology models

The ontological relationships between the terms in the reference guide are captured in these ontology models.

The first model describes the relationships between information about mutations and the physical mutations themselves, which are located within a genome of some organism.  This model is both flexible and robust enough to work with different variant naming conventions. Entities outlined in orange are captured in the DataHarmonizer template.
![mutation model](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/blob/main/img/mutations.drawio.png)

The second model describes one or more mutation symbols that are correlated with a functional effect, as reported in the literature. 
![evidence model](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/blob/main/img/evidence.drawio.png)

## Contacts
For more information and/or assistance, contact Madeline Iseminger at miseming at sfu dot ca or submit a repository [issue request](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/issues).

## License

[MIT License](https://github.com/cidgoh/pathogen-mutation-functionalannotation-package/blob/main/LICENSE)

## Acknowledgements

Brought to you by The [Centre for Infectious disease Genomics and One Health](https://cidgoh.ca/).

![LogoCIDGOH2](https://github.com/cidgoh/specification-repo-template/assets/48695054/87fa713d-8fd7-453d-8542-fc413069e842)
