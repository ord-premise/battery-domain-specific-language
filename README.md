# D3.3 -  Domain-specific language for battery assembly and testing, and its implementation in a hardware scheduler

A domain-specific language (DSL) can be regarded as a standardized language that allows different stakeholders (in this case, battery researchers from various research groups and institutions) to communicate concepts in battery assembly unambiguously. A DSL is crucial for ensuring interoperability in battery research across diverse groups and institutions. One practical approach to facilitating a DSL in battery assembly and testing is to semantically annotate terms used in these processes to meaningful ontologies. See [here](https://github.com/ord-premise/interoperability-guidelines) for more details on ontologizing metadata. However, the burden of semantically annotating data and/or metadata typically outweighs the perceived benefits of interoperability for individual researchers. We previously created example coin cell battery assembly schemas in .xlsx and a Python script to convert the .xlsx schema into ontologized battery assembly metadata in JSON-LD (available [here](https://github.com/ord-premise/metadata-batteries)).  In this deliverable, we expand the capability of this .xlsx schema to cover the metadata for battery testing. We also improve the conversion script, allowing the .xlsx schema to be applicable with different battery chemistries and cell configurations. In addition to this, we also provide an example of how the ontologized battery metadata can be integrated with our battery cyclers.


## Authors

- Nukorn Plainpan (Empa, Switzerland)
- Corsin Battaglia (Empa, Switzeralnd) 

## Goal

To provide a tool that enables individual researchers to semantically annotate their battery assembly and testing metadata using the BattINFO ontology developed by the Battery 2030+ consortium, and to demonstrate how this tool is integrated into battery cyclers.  


## Achievement

We have upgraded the .xlsx schema to now cover the metadata for battery testing. We also upgraded our Python script for converting .xlsx schema to JSON-LD into a Python-based web application, namely the [BattINFO converter](https://battinfoconverter.streamlit.app/). This web application allows the user to convert .xlsx schemas to JSON-LD documents without the need to install Python on the local machine, lowering the barrier to entry for non-technical users. BattINFO converter also allows users to modify the .xlsx schemas to suit the battery chemistry of their choice, thus allowing an even larger audience to apply the DSL in their research. The documentation on how to use BattINFO converter and customize .xlsx schemas is provided on the BattINFO converter page. The philosophy behind the BattINFO converter is detailed in an article submitted to the journal of Batteries & Supercaps for peer review and is currently in revision. We are presently integrating the BattINFO converter into a battery cycling pipeline at Empa.


## External links

- [BattINFO converter webapp](https://battinfoconverter.streamlit.app/)  
- [BattINFO converter repo](https://github.com/EmpaEconversion/BattInfoConverter)  
- [BattINFO ontology repo](https://github.com/BIG-MAP/BattINFO)

## Acknowledgements

The [PREMISE](https://ord-premise.org/) project is supported by the [Open Research Data Program](https://ethrat.ch/en/eth-domain/open-research-data/) of the ETH Board.

![image](https://ord-premise.org/assets/img/logos/PREMISE-logo.svg)

![image](https://ethrat.ch/wp-content/uploads/2021/12/ethr_en_rgb_black.svg)
