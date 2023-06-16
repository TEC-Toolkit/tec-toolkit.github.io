---
layout: default
---

[back to main page](./)

# Getting started
In this page we provide an overview of the entry points for using the TEC-Toolkit resources. [ECFO](/#the-emission-conversion-factor-ontology-ecfo) and [PECO](/#the-provenance-of-emission-calculations-ontology-peco) ontologies may be use together or separately. For example, the [Emissions Conversion Factors KG](/#emissions-conversion-factors) uses ECFO and can be used as a look up database of conversion factors (see [how below](/#retrieve-a-conversion-factor)). 

PECO may be used to describe the emission calculation process, which typically also involves the conversion factors and hence the combination of PECO and ECFO may be desired. Semantic Machine Learning Impact calculator is a prototype software that demonstrates how PECO and Emissions Conversion Factors KG can be embedded within a web-based application [see how can you donwload a PECO trace](/#download-a-peco-trace). 

For further information on ECFO and PECO follow the w3id link that will let you download the ontologies and/or view the online documentation. 

Please see the [SMLI Calculator](/#smli-calculator) for a link to online demo and source code to further explore how the individual components of the TEC toolkit might be integrated in a software application.

## Retrieve an Emission Conversion Factor (ECF) Metadata 

The simplest way of browsing the metadata of an emission factor is just pasting its URI in a browser. For example, [https://w3id.org/ecfkg/i/UK/BEIS/2019/CF_1](https://w3id.org/ecfkg/i/UK/BEIS/2019/CF_1) will take you to an online page like this one: 


![rdf_explorer](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/3984bfc1-0167-42bf-b609-d77c38b3f187)

where you can see the units, value and source (among others) of the emission conversion factor. However, how to get to the ECF URI? One way of doing it is using SPARQL queries. We have set up a simple [SPARQL query interface](https://query.cf.linkeddata.es/query) where you can create SPARQL queries and retrieve the ids of the ECFs you may be interested in. For example, to retrieve ECFs related to "Butane" in 2020, just issue the following query:

````
TO DO
````

The results will include several ECFS, make sure you read their details before selecting the one of interest:
```
TO DO show results
```

## Plotting the evolution of an Emission Conversion Factor 

Point to the notebook where a more detailed analysis can be seen. Show the picture of the plot. Put the notebooks online

## PECO trace

* To test an example provenance trace of emission calculations use this [TTL file](https://github.com/TEC-Toolkit/PECO/blob/main/cqs/provenance_trace.ttl).

* See [here](https://github.com/TEC-Toolkit/PECO/blob/main/cqs/README.md) for a list of example SPARQL queries that can be run on this data.

For example, this query will retrieve the emission score and the activity for which this  score was calculated: 
  ```
PREFIX ecfo: <https://w3id.org/ecfo#>  
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> 
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#> 
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>  
PREFIX prov:<http://www.w3.org/ns/prov#> 
PREFIX qudt: <http://qudt.org/schema/qudt/>

Select ?activityL ?score
Where {
    ?activity  rdf:type   peco:EmissionGenerationActivity ;
               rdfs:label ?activityL;
               peco:hasEmissionScore/qudt:value ?score.    
}
  ```

* You can also run it online in our sample [Colab notebook](https://colab.research.google.com/drive/1wl9xA-0HQ5aWI-u517gC1ZwsC10eJZQa?usp=sharing).


## Ontologies

### The Emission Conversion Factor Ontology (ECFO)

![ECFO Logo](https://raw.githubusercontent.com/TEC-Toolkit/tec-toolkit.github.io/main/assets/Logo%20ECFO.svg){: width="5%"}

Available at: [https://w3id.org/ecfo](https://w3id.org/ecfo)

Evalaution & Examples: [CQs and SPARQL queries](https://github.com/TEC-Toolkit/PECO/tree/main/cqs)

Aims to provide a generic model for describing the values of Emission Conversion Factors and their associated metadata.

![ecfo](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/c352e7e3-8bd8-4391-be94-a36e406cfee6)


### The Provenance of Emission Calculations Ontology (PECO)

 ![PECO Logo](https://raw.githubusercontent.com/TEC-Toolkit/tec-toolkit.github.io/main/assets/Logo%20PECO.svg){: width="5%"}

Available at: [https://w3id.org/peco](https://w3id.org/peco)

Evalaution & Examples: [CQs and SPARQL queries](https://github.com/TEC-Toolkit/ECFO/tree/main/cqs)

Defines a vocabulary for describing provenance traces of carbon emissions calculations by capturing the quantifiable measurements of energy estimates (i.e., activity data and emission conversion factors used to estimate the carbon emissions).

![peco](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/ee9de0fa-8191-4226-a6f5-cddc423ed192)


## Emissions Conversion Factors KG

* [SPARQL endpoint](https://sparql.cf.linkeddata.es/cf/). See [https://github.com/TEC-Toolkit/cfkg#sparql-endpoint](https://github.com/TEC-Toolkit/cfkg#sparql-endpoint) to learn more on doing queries.
* [Knowledge Graph in Turtle](https://zenodo.org/record/7916096#.ZFugTo1BxEY)

Emission Conversion Factors described using ECFO [GitHub repository](https://github.com/TEC-Toolkit/cfkg): 

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

### Additional Sample queries
TO DO (separate page)

## Software

### SMLI Calculator

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

Together with the calculated emission score, the GUI also shows detailed information about the activities performed during the calculation process, the conversion factor used and other relevant conversion factors that are applicable to the user input: 

![result](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/8c49385b-43d3-443c-ab2a-af2256995648)


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
The results are presented in the GUI: 

![validation](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/92f8272a-5b65-4274-9045-9a2143edd794)

The provenance trace can be also downloaded by the user. 

![download_trace](https://github.com/TEC-Toolkit/tec-toolkit.github.io/assets/4025828/a7f2088b-e2b2-4eca-b395-a753e0140ffb)


For expanded example of provenance trace and additional queries please see [our competency questions](https://github.com/TEC-Toolkit/PECO/tree/main/cqs)


### Data Validation

The [Data Validation component](https://github.com/TEC-Toolkit/Data-Validation) runs Datalog rules to detect violations of conditions according to ECFO.

[back to main page](./)
