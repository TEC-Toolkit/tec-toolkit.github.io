![TEC logo](Logo TEC.svg)

# About

With the Net Zero agenda gaining significant traction across the world, organisations are often required to report carbon emissions associated with their operation. However, calculating emissions is not a trivial task and reported scores can differ depending on the choices made by those performing the calculations or the software used to assist with this task. This might include the methodology and conversion factors used to calculate the scores as well as the origin and accuracy of the input data (e.g., energy usage). 
The aim of this project and this open source initiative is to provide ontology models and software tools to formalise provenance of carbon footprint calculations in a machine-understandable knowledge graphs to enhance the transparency of such process. We argue that such provenance metadata is crucial in supporting assessments of emission scores' veracity and trustworthiness, as well as improving the understandability of the calculated scores so they can be meaningfully integrated with other results across the supply chains.

## Team

* [Milan Markovic](https://orcid.org/0000-0002-5477-287X), Interdisciplinary Centre for Data and AI, [University of Aberdeen](https://www.abdn.ac.uk/)
* [Daniel Garijo](https://orcid.org/0000-0003-0454-7145), Ontology Engineering Group, [Universidad Politécnica de Madrid](https://www.upm.es/)
* [Stefano Germano](https://orcid.org/0000-0001-6993-0618), Department of Computer Science, [University of Oxford](https://www.ox.ac.uk/)
* [Iman Naja](https://orcid.org/0000-0001-6634-3266), Knowledge Media Institute, [The Open University](https://www.open.ac.uk/)

## Cite as

Milan Markovic, Daniel Garijo, Stefano Germano and Iman Naja. Transparent Emission Calculations (TEC) Toolkit. 2023. URL: https://tec-toolkit.github.io/ 

## License
The license for the TEC toolkit is [CC-BY 4.0]{http://creativecommons.org/licenses/by/4.0}. All its components are under the same license except for the Semantic Machine Lerning Impact Calculator which is under the MIT License (MIT). 

# Resources

The TEC toolkit consists ontologies for modelling ECFs in KGs and describing provenance traces of emissions calculations, public Knowledge Graphs built from open data with over 42400 ECFs, and the Semantic Machine Lerning Impact Calculator.

## Ontologies 

* The Emission Conversion Factor Ontology (ECFO) - [https://w3id.org/ecfo](https://w3id.org/ecfo)- aims to provide a generic model for describing the values of Emission Converstion Factors and their associated metedata.
* The Provenance of Emission Calculations Ontoltogy (PECO) - [https://w3id.org/peco](https://w3id.org/peco) - defines a vocabulary for describing provenance traces of carbon emissions calculations by capturing the quantifiable measurements of energy estimates, i.e., activity data (e.g., electricity used by a machinery to produce a product, petrol used to make a car journey, etc.) and emission conversion factors used to estimate the carbon emissions.

## Knowledge Graphs 

* [SPARQL endpoint](https://cf.linkeddata.es/sparql)

* Emission Conversion Factors described using ECFO [GITHUB repo](https://github.com/TEC-Toolkit/cfkg)
 
| Year        | Publisher | Country  | Description      | Number of Conversion Factors |
|:-------------|:------- |:-------|  :------------------| :-------|
| 2016 -2022     | BEIS | UK | These emission conversion factors are for use by UK and international organisations to report on greenhouse gas emissions. | 42400 | 

## Software

The [Semantic Machine Lerning Impact Calculator](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator) is an extension of the [Machine learning Impact (MLI) calculator](https://mlco2.github.io/impact\#compute) with semantic components to perform the emission calculations.

The [Data Validation component](https://github.com/TEC-Toolkit/Data-Validation) which runs Datalog rules to detect violations of conditions.
