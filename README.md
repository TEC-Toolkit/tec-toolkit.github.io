<div style="text-align: center">

<img src="assets/Logo%20TEC.svg" alt="TEC-Toolkit Logo" width=10% />

</div>

# TEC-Toolkit
The website of the TEC-Toolkit is available at https://w3id.org/tec-toolkit/

With the Net Zero agenda gaining significant traction across the world, organisations are often required to report carbon emissions associated with their operation. However, calculating emissions is not a trivial task and reported scores can differ depending on the choices made by those performing the calculations or the software used to assist with this task. This might include the methodology and conversion factors used to calculate the scores as well as the origin and accuracy of the input data (e.g., energy usage).
The aim of this project and this open source initiative is to provide ontology models and software tools to formalise provenance of carbon footprint calculations in a machine-understandable knowledge graphs to enhance the transparency of such process. We argue that such provenance metadata is crucial in supporting assessments of emission scores' veracity and trustworthiness, as well as improving the understandability of the calculated scores so they can be meaningfully integrated with other results across the supply chains.

# Team

* [Milan Markovic](https://orcid.org/0000-0002-5477-287X), Interdisciplinary Centre for Data and AI, [University of Aberdeen](https://www.abdn.ac.uk/)
* [Daniel Garijo](https://orcid.org/0000-0003-0454-7145), Ontology Engineering Group, [Universidad Politécnica de Madrid](https://www.upm.es/)
* [Stefano Germano](https://orcid.org/0000-0001-6993-0618), Department of Computer Science, [University of Oxford](https://www.ox.ac.uk/)
* [Iman Naja](https://orcid.org/0000-0001-6634-3266), Knowledge Media Institute, [The Open University](https://www.open.ac.uk/)

# Cite as

> Milan Markovic, Daniel Garijo, Stefano Germano and Iman Naja. Transparent Emission Calculations (TEC) Toolkit. 2023. URL: https://tec-toolkit.github.io

The TEC toolkit is composed of different resources (KGs, tools, data). If you use a particular one, please cite it appropriately with its corresponding DOI

# License

The license for the TEC toolkit is [CC-BY 4.0](http://creativecommons.org/licenses/by/4.0).
See the [LICENSE](LICENSE) file for details.

Note that the TEC toolkits components have different licenses.
Please refer to the LICENSE files in the specific components to know more about them (e.g., datasets).

# Resources

* [Emission Conversion Factors Ontology](https://github.com/TEC-Toolkit/ECFO): Repository of an ontology that formalises emission conversion factors.
* [Provenance of Emission Calculation Ontology](https://github.com/TEC-Toolkit/peco): Repository of an ontology extending the PROV standard with the traces of emission calculations.
* [Conversion Factors Knowledge Graph](https://github.com/TEC-Toolkit/cfkg): Repository with the mappings, cleaning steps and sources used to generate a knowledge graph of conversion factors.
* [Conversion factor SPARQL endpoint](https://query.cf.linkeddata.es/query): SPARQL endpoint query interface with the current conversion factors loaded. The sparql endpoint itself is available [here](https://sparql.cf.linkeddata.es/).
* [Data validation module](https://github.com/TEC-Toolkit/Data-Validation): Repository for the module that performs data validation using Datalog.
* [Semantic Machine Learning Impact Calculator (SMLIC)](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator): Repository for the code and queries used to create a transparent emission calculator, together with a fully transparent emission report. This repo also links to the [Demo](https://calculator.linkeddata.es/).
