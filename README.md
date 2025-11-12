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

##  How to Use SMEDG Ontology

###  1. Using in **Stardog**
1. Open **Stardog Studio** or **Stardog Designer**.
2. Create a new database (e.g., `smedg_db`).
3. Click **Add Data → Import RDF** and upload:
   - `Model/smedg_ontology.ttl`
   - `SHACL_Shapes/smedg_shapes.ttl`
   - (Optionally) `Data/sample_dataset.ttl`
4. To run validation:
   - In Stardog Studio, open the **SHACL Validation** tab.
   - Select your shapes graph and click **Run Validation**.
   - Review alerts and validation results in the results panel.
5. To execute SPARQL queries:
   - Open the **SPARQL Editor** and load queries from `SPARQL_Queries/`.
   - Run enforcement or monitoring queries directly on the dataset.

---

###  2. Using in **Protégé**
1. Download and install [Protégé](https://protege.stanford.edu/).
2. Go to **File → Open** and select `Model/smedg_ontology.ttl`.
3. Use the **Entities** and **Object Properties** tabs to explore the model structure.
4. You can validate instances manually or use plugins like **SHACLTab** for SHACL validation.
5. To visualise relationships:
   - Go to **Reasoner → Start reasoner → HermiT or Pellet**
   - Open the **OntoGraf** tab to see class relationships visually.

---

###  3. Reuse and Extension
- You can extend the ontology by adding new policies, classes, or shapes.
- For consistency, follow the same namespace used in the current files:


## License

Released under the **MIT License**. You are free to reuse, modify, and extend this ontology with proper attribution and refrence.



**Contact:**  
Bushra Al Sulayyim  
University of Technology Sydney (UTS)
bushra.alsulayyim@uts.edu.au

