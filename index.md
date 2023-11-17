<!-- <div style="width:30%">

![TEC-Toolkit Logo](assets/Logo%20TEC.svg| width=100)

</div> -->

 ![TEC Logo](https://raw.githubusercontent.com/TEC-Toolkit/tec-toolkit.github.io/main/assets/Logo%20TEC.svg){: width="10%"}

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

> Markovic, M., Garijo, D., Germano, S., Naja, I. (2023). TEC: Transparent Emissions Calculation Toolkit. In: Payne, T.R., et al. The Semantic Web – ISWC 2023. ISWC 2023. Lecture Notes in Computer Science, vol 14266. Springer, Cham. https://doi.org/10.1007/978-3-031-47243-5_5

## License

The license for the TEC toolkit ontologies is [CC-BY 4.0](http://creativecommons.org/licenses/by/4.0).
For the software components, the [Semantic Machine Lerning Impact Calculator](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator) and the [data validation module](https://github.com/TEC-Toolkit/Data-Validation) are under the MIT License (MIT).
The [mappings and KG](https://github.com/EATS-UoA/cfkg) are under an Apache 2.0 license.

# Presentations

- Slides from the the 22nd International Semantic Web Conference 2023 [slides](https://github.com/TEC-Toolkit/tec-toolkit.github.io/files/13377520/ISWC.2023.pdf)


# Resources
The TEC Toolkit includes the resources listed below. Every resource has its own GitHub repository, available in the [TEC-Toolkit organization](https://github.com/TEC-Toolkit):

## Ontologies
- [ECFO](https://w3id.org/ecfo) aims to provide a generic model for describing the values of Emission Conversion Factors and their associated metadata. 
- [PECO](https://w3id.org/peco) defines a vocabulary for describing provenance traces of carbon emissions calculations by capturing the quantifiable measurements of energy estimates (i.e., activity data and emission conversion factors used to estimate the carbon emissions).  

## Knowledge Graph
The Emission Conversion Factor Knowledge Graph (based on ECFO) contains over 40.000 conversion factors from two different sources over 2002-2022
- [Knowledge Graph query interface](https://query.cf.linkeddata.es/query)
- [SPARQL query examples](https://github.com/TEC-Toolkit/cfkg#sparql-endpoint) to learn more on doing queries.

## Software
- The [Semantic Machine Lerning Impact Calculator](https://calculator.linkeddata.es) (please open it in Chrome) is an extension of the [Machine learning Impact (MLI) calculator](https://mlco2.github.io/impact\#compute) with semantic components to perform the emission calculations.
- The [Data Validation component](https://github.com/TEC-Toolkit/Data-Validation) runs Datalog rules to detect violations of conditions according to ECFO.

# Getting started
Please see our [project documentation](./getting_started.html) for more information about searching and working with Emission Conversion Factors, how to download and query provenance traces, how to perform validation queries and how to use the ontologies.


## Acknowledgments 

This work was supported by eBay, Samsung Research UK, Siemens AG, the EPSRC projects ConCur (EP/V050869/1), UK FIRES (EP/S019111/1) and EATS (EP/V042270/1), the EU Horizon 2020 project GATEKEEPER (No 857223) and by the Comunidad de Madrid under the Multiannual Agreement with Universidad Politécnica de Madrid (UPM) in the line Support for R\&D projects for Beatriz Galindo researchers, in the context of the V PRICIT (Regional Programme of Research and Technological Innovation) and through the call Research Grants for Young Investigators from UPM.
