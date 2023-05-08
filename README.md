# TEC-Toolkit

With the Net Zero agenda gaining significant traction across the world, organisations are often required to report carbon emissions associated with their operation. However, calculating emissions is not a trivial task and reported scores can differ depending on the choices made by those performing the calculations or the software used to assist with this task. This might include the methodology and conversion factors used to calculate the scores as well as the origin and accuracy of the input data (e.g., energy usage). 
The aim of this project and this open source initiative is to provide ontology models and software tools to formalise provenance of carbon footprint calculations in a machine-understandable knowledge graphs to enhance the transparency of such process. We argue that such provenance metadata is crucial in supporting assessments of emission scores' veracity and trustworthiness, as well as improving the understandability of the calculated scores so they can be meaningfully integrated with other results across the supply chains.

# Team

* [Milan Markovic](https://orcid.org/0000-0002-5477-287X), Interdisciplinary Centre for Data and AI, [University of Aberdeen](https://www.abdn.ac.uk/)
* [Daniel Garijo](https://orcid.org/0000-0003-0454-7145), Ontology Engineering Group, [Universidad Politécnica de Madrid](https://www.upm.es/)
* [Stefano Germano](https://orcid.org/0000-0001-6993-0618), Department of Computer Science, [University of Oxford](https://www.ox.ac.uk/)
* [Iman Naja](https://orcid.org/0000-0001-6634-3266), Knowledge Media Institute, [The Open University](https://www.open.ac.uk/)

# Cite as

Milan Markovic, Daniel Garijo, Stefano Germano and Iman Naja. Transparent Emission Calculations (TEC) Toolkit. 2023. URL: https://tec-toolkit.github.io/ 

# License
The license for the TEC toolkit is [CC-BY 4.0][http://creativecommons.org/licenses/by/4.0] - - see the [LICENSE](LICENSE) file for details.
Note that all the TEC toolkits components are under the same license except for the Semantic Machine Lerning Impact Calculator which is under the MIT License (MIT). 

# Resources

* [Emission Conversion Factors Ontology](https://github.com/EATS-UoA/ECFO): Repository of an ontology that formalises emission conversion factors.
* [Provenance of Emission Calculation Ontology](https://github.com/EATS-UoA/peco): Repository of an ontology extending the PROV standard with the traces of emission calculations.
* [Conversion Factors Knowledge Graph](https://github.com/EATS-UoA/cfkg): Repository with the mappings, cleaning steps and sources used to generate a knowledge graph of conversion factors.
* [Conversion factor SPARQL endpoint](https://sparql.cf.linkeddata.es/): SPARQL endpoint with the current conversion factors loaded.
* [Data validation module](https://github.com/TEC-Toolkit/Data-Validation): Repository for the module that performs data validation using Datalog.
* [Semantic Machine Learning Impact Calculator (SMLIC)](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator): Repository for the code and queries used to create a transparent emission calculator, together with a fully transparent emission report. This repo also links to the [Demo](https://calculator.linkeddata.es/).
