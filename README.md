# SMEDG (SME Data Governance)
**Ontology-driven policy enforcement and monitoring for SME Information Governance**

This repository hosts the core artefacts developed as part of the **SMEDG (SME-Data Governance)** framework, a knowledge-graph-based approach for automating data governance, compliance validation, and monitoring in small to medium enterprises (SMEs).

## 📂 Repository Structure

| Folder | Description |
|---------|--------------|
| **Model/** | Contains the SMEDG ontology model (`.ttl`) defining classes, properties, and relationships. |
| **SHACL_Shapes/** | Includes SHACL shapes used for policy validation and compliance checking. |
| **SPARQL_Queries/** | Contains SPARQL queries and rules for policy enforcement, monitoring, and alert generation. |
| **Data/** | Example or synthetic datasets used for testing and evaluating the ontology and SHACL rules. |

## Overview

SMEDG provides a lightweight, ontology-based framework designed to:
- Encode information governance (data classification) and compliance rules as executable knowledge-graph constraints  
- Automate validation and alerting through SHACL and SPARQL  
- Support transparent, human-readable monitoring for non-technical SME users  

The ontology is compatible with RDF-compliant systems such as **Stardog**, **Protégé**, and **GraphDB**.



## License

Released under the **MIT License**. You are free to reuse, modify, and extend this ontology with proper attribution and refrence.



**Contact:**  
Bushra Al Sulayyim  
University of Technology Sydney (UTS)
bushra.alsulayyim@uts.edu.au

