<!-- <div style="width:30%">

![TEC-Toolkit Logo](assets/Logo%20TEC.svg)

</div> -->

# About

With the Net Zero agenda gaining significant traction across the world, organisations are often required to report carbon emissions associated with their operation. However, calculating emissions is not a trivial task and reported scores can differ depending on the choices made by those performing the calculations or the software used to assist with this task. This might include the methodology and conversion factors used to calculate the scores as well as the origin and accuracy of the input data (e.g., energy usage).
The aim of this project and this open source initiative is to provide ontology models and software tools to formalise provenance of carbon footprint calculations in a machine-understandable knowledge graphs to enhance the transparency of such process. We argue that such provenance metadata is crucial in supporting assessments of emission scores' veracity and trustworthiness, as well as improving the understandability of the calculated scores so they can be meaningfully integrated with other results across the supply chains.

The TEC toolkit consists ontologies for modelling ECFs in KGs and describing provenance traces of emissions calculations, public Knowledge Graphs built from open data with over 42400 ECFs, and the Semantic Machine Lerning Impact Calculator.

## Team

* [Milan Markovic](https://orcid.org/0000-0002-5477-287X), Interdisciplinary Centre for Data and AI, [University of Aberdeen](https://www.abdn.ac.uk/)
* [Daniel Garijo](https://orcid.org/0000-0003-0454-7145), Ontology Engineering Group, [Universidad Politécnica de Madrid](https://www.upm.es/)
* [Stefano Germano](https://orcid.org/0000-0001-6993-0618), Department of Computer Science, [University of Oxford](https://www.ox.ac.uk/)
* [Iman Naja](https://orcid.org/0000-0001-6634-3266), Knowledge Media Institute, [The Open University](https://www.open.ac.uk/)

## Cite as

> Milan Markovic, Daniel Garijo, Stefano Germano and Iman Naja. Transparent Emission Calculations (TEC) Toolkit. 2023. URL: [https://w3id.org/tec-toolkit/](https://w3id.org/tec-toolkit/)

## License

The license for the TEC toolkit ontologies is [CC-BY 4.0](http://creativecommons.org/licenses/by/4.0).
For the software components, the [Semantic Machine Lerning Impact Calculator](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator) and the [data validation module](https://github.com/TEC-Toolkit/Data-Validation) are under the MIT License (MIT).
The [mappings and KG](https://github.com/EATS-UoA/cfkg) are under an Apache 2.0 license.

# How to Use this Resource

TBA






# Ontologies

## The Emission Conversion Factor Ontology (ECFO)

<!-- <img src="assets/Logo%20ECFO.svg" alt="ECFO Logo" width=20% /> -->

Available at: [https://w3id.org/ecfo](https://w3id.org/ecfo)

Aims to provide a generic model for describing the values of Emission Conversion Factors and their associated metadata.

![ecfo](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/c352e7e3-8bd8-4391-be94-a36e406cfee6)



## The Provenance of Emission Calculations Ontoltogy (PECO)

<!-- <img src="assets/Logo%20PECO.svg" alt="PECO Logo" width=20% /> -->

Available at: [https://w3id.org/peco](https://w3id.org/peco)

Defines a vocabulary for describing provenance traces of carbon emissions calculations by capturing the quantifiable measurements of energy estimates (i.e., activity data and emission conversion factors used to estimate the carbon emissions).

![peco](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/ee9de0fa-8191-4226-a6f5-cddc423ed192)

# Knowledge Graphs

## Emissions Conversion Factors

* [SPARQL endpoint](https://sparql.cf.linkeddata.es/cf/). See [https://github.com/TEC-Toolkit/cfkg#sparql-endpoint](https://github.com/TEC-Toolkit/cfkg#sparql-endpoint) to learn more on doing queries.
* [Knowledge Graph in Turtle](https://zenodo.org/record/7916096#.ZFugTo1BxEY)

* Emission Conversion Factors described using ECFO [GitHub repo](https://github.com/TEC-Toolkit/cfkg)

| Year       | Publisher                                                                                                        | Country | Description                                                                                                                       | Number of Conversion Factors |
| :--------- | :--------------------------------------------------------------------------------------------------------------- | :------ | :-------------------------------------------------------------------------------------------------------------------------------- | :--------------------------- |
| 2022       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 6464                         |
| 2021       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 6284                         |
| 2020       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 6140                         |
| 2019       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 6163                         |
| 2018       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 6192                         |
| 2017       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 6178                         |
| 2016       | <a href="https://www.gov.uk/government/collections/government-conversion-factors-for-company-reporting">BEIS</a> | UK      | Official list of emission conversion factors for use by UK and international organisations to report on greenhouse gas emissions. | 4977                         |
| 2002 -2019 | <a href="https://github.com/mlco2/impact">MLI</a>                                                                | Various | A collection of Scope 2 electricity emission conversion factors from a range of sources.                                          | 81                           |

# Software

## SMLI Calculator

The [Semantic Machine Lerning Impact Calculator](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator) is an extension of the [Machine learning Impact (MLI) calculator](https://mlco2.github.io/impact\#compute) with semantic components to perform the emission calculations.

***SMLI Demo*** 

https://calculator.linkeddata.es  
(currently only Chrome is supported)

## Data Validation

The [Data Validation component](https://github.com/TEC-Toolkit/Data-Validation) runs Datalog rules to detect violations of conditions according to ECFO.
