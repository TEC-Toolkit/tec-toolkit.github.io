<!-- <div style="width:30%">

![TEC-Toolkit Logo](assets/Logo%20TEC.svg| width=200)

</div> -->

 ![TEC Logo](https://raw.githubusercontent.com/TEC-Toolkit/tec-toolkit.github.io/main/assets/Logo%20TEC.svg|width=200)

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

[ECFO](/#the-emission-conversion-factor-ontology-ecfo) and [PECO](/#the-provenance-of-emission-calculations-ontology-peco) ontologies may be use together or separately. For example, the [Emissions Conversion Factors KG](/#emissions-conversion-factors) uses ECFO and can be used as a look up database of conversion factors. 

PECO may be used to describe the emission calculation process, which typically also involves the conversion factors and hence the combination of PECO and ECFO may be desired. Semantic Machine Learning Impact calculator is a prototype software that demonstrates how PECO and Emissions Conversion Factors KG can be embedded within a web-based application. 

For further information on ECFO and PECO follow the w3id link that will let you download the ontologies and/or view the online documentation. 

Please see the [SMLI Calculator](/#smli-calculator) for a link to online demo and source code to further explore how the individual components of the TEC toolkit might be integrated in a software application.




# Ontologies

## The Emission Conversion Factor Ontology (ECFO)

![ECFO Logo](https://raw.githubusercontent.com/TEC-Toolkit/tec-toolkit.github.io/main/assets/Logo%20ECFO.svg|width=200)

Available at: [https://w3id.org/ecfo](https://w3id.org/ecfo)

Evalaution & Examples: [CQs and SPARQL queries](https://github.com/TEC-Toolkit/PECO/tree/main/cqs)

Aims to provide a generic model for describing the values of Emission Conversion Factors and their associated metadata.

![ecfo](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/c352e7e3-8bd8-4391-be94-a36e406cfee6)



## The Provenance of Emission Calculations Ontology (PECO)

 ![PECO Logo](https://raw.githubusercontent.com/TEC-Toolkit/tec-toolkit.github.io/main/assets/Logo%20PECO.svg|width=200)

Available at: [https://w3id.org/peco](https://w3id.org/peco)

Evalaution & Examples: [CQs and SPARQL queries](https://github.com/TEC-Toolkit/ECFO/tree/main/cqs)

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


***How it works*** 

SMLI Calculator queries the live ECFO KG to retrieve the information about the available conversion factors that match the user input. 

An example call to [Java-based backend](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator/blob/main/src/main/java/io/github/tectoolkit/calculator/Controller.java) that queries the ECFO KG for corresponding conversion factors:

````
fetch('/cf_info_all?region=' + region)
		.then((response) =>
			response.json()
		)
		.then((CF_data) => {
			
			....
			
			})
````


A SPARQL query executed to retrieve conversion factors for a specific region of compute: 
````
PREFIX  geo:  <http://www.opengis.net/ont/geosparql#>
PREFIX  qudt: <http://qudt.org/schema/qudt/>
PREFIX  peco: <https://w3id.org/peco#>
PREFIX  rdf:  <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX  owl:  <http://www.w3.org/2002/07/owl#>
PREFIX  ecfo: <https://w3id.org/ecfo#>
PREFIX  xsd:  <http://www.w3.org/2001/XMLSchema#>
PREFIX  rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX  time: <http://www.w3.org/2006/time#>
PREFIX  prov: <http://www.w3.org/ns/prov#>

SELECT DISTINCT  ?id ?sourceUnit ?targetUnit ?source ?value ?applicableLocation ?applicablePeriodStart ?applicablePeriodEnd ?emissionTargetSymbol
WHERE
  { ?id       rdf:type            ecfo:EmissionConversionFactor ;
              ecfo:hasTargetUnit  ?targetUnitInst .
    ?targetUnitInst
              rdfs:label          "kilogram"@en .
    ?id ecfo:hasEmissionTarget/rdfs:label ?emissionTargetSymbol
      { ?id ecfo:hasApplicableLocation/rdfs:label "europe-west2"@en }
    UNION
      { ?id (ecfo:hasApplicableLocation/geo:ehContains)/rdfs:label "europe-west2"@en .
        ?id  ecfo:hasScope         ecfo:Scope2 ;
             ecfo:hasTag           <https://w3id.org/ecfkg/i/UK%20electricity> ;
             ecfo:hasEmissionTarget  <http://www.wikidata.org/entity/Q1933140>
      }
    OPTIONAL
      { ?id  ecfo:hasSourceUnit  ?sourceUnitInst }
    OPTIONAL
      { ?id  ecfo:hasApplicableLocation  ?location }
    OPTIONAL
      { ?id (ecfo:hasApplicablePeriod/time:hasBeginning)/time:inXSDDate ?applicablePeriodStart }
    OPTIONAL
      { ?id (ecfo:hasApplicablePeriod/time:hasEnd)/time:inXSDDate ?applicablePeriodEnd }
    OPTIONAL
      { ?id  prov:wasDerivedFrom  ?source }
    OPTIONAL
      { ?id  rdf:value  ?value }
    OPTIONAL
      { ?location  rdfs:label  ?applicableLocation }
    OPTIONAL
      { ?targetUnitInst
                  qudt:abbreviation  ?targetUnit
      }
    OPTIONAL
      { ?sourceUnitInst
                  qudt:abbreviation  ?sourceUnit
      }
  }
ORDER BY DESC(?applicablePeriodEnd)
````

The calculator also produces JSON-LD descriptions of provenance traces documenting the individual steps of emissions calculation process. [JSON-LD context](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator/blob/main/src/main/resources/static/js/tec-context.js) and set of custom [JavaScript Functions](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator/blob/main/src/main/resources/static/js/tec-lib.js) are used to query ECFO KG to retrieve the information about the Emission Conversion Factors and to generate portion of the provenance trace. 

An example of generating description of activity with a connected input entity in the [code that calculates the emissions](https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator/blob/main/src/main/resources/static/js/grayscale.js): 

````
	let wattConsumption = createCalculationEntity("Watt Consumption", state.gpus[gpu].watt, "http://www.wikidata.org/entity/Q25236", "http://www.wikidata.org/entity/Q1053879", graphLD, "")
	
	let electricityUseEstimate = createCalculationActivity("https://github.com/TEC-Toolkit/Semantic_Machine_Learning_Impact_Calculator", "Estimate Electricity Use in kW/h", graphLD)
	
	linkInputEntityToActivity(wattConsumption, electricityUseEstimate, graphLD)
````

The calculator also executes a number of validation queries, for example, to check if the latest available conversion factor is up to date: 

````
PREFIX  geo:  <http://www.opengis.net/ont/geosparql#>
PREFIX  qudt: <http://qudt.org/schema/qudt/>
PREFIX  peco: <https://w3id.org/peco#>
PREFIX  rdf:  <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX  owl:  <http://www.w3.org/2002/07/owl#>
PREFIX  ecfo: <https://w3id.org/ecfo#>
PREFIX  xsd:  <http://www.w3.org/2001/XMLSchema#>
PREFIX  rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX  time: <http://www.w3.org/2006/time#>
PREFIX  prov: <http://www.w3.org/ns/prov#>

SELECT DISTINCT  ?cf ?cf_value ?time
WHERE
  { ?entity  rdf:type  peco:EmissionScore .
    ?entity prov:wasGeneratedBy/prov:used ?cf .
    ?cf (ecfo:hasApplicablePeriod/time:hasEnd)/time:inXSDDate ?time .
    ?cf  rdf:value  ?cf_value
    FILTER ( ?time < now() )
  }
````

The provenance trace can be also downloaded by the user. 


For expanded example of provenance trace and additional queries please see [here](https://github.com/TEC-Toolkit/PECO/tree/main/cqs)


## Data Validation

The [Data Validation component](https://github.com/TEC-Toolkit/Data-Validation) runs Datalog rules to detect violations of conditions according to ECFO.

# Acknowledgments 

This work was supported by eBay, Samsung Research UK, Siemens AG, the EPSRC projects ConCur (EP/V050869/1), UK FIRES (EP/S019111/1) and EATS (EP/V042270/1), the EU Horizon 2020 project GATEKEEPER (No 857223) and by the Comunidad de Madrid under the Multiannual Agreement with Universidad Politécnica de Madrid (UPM) in the line Support for R\&D projects for Beatriz Galindo researchers, in the context of the V PRICIT (Regional Programme of Research and Technological Innovation) and through the call Research Grants for Young Investigators from UPM.
