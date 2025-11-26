## Tables

### **Online Appendix Table 1: Policy Rules Extracted from the Information Security Guide**
This table lists all 48 policy rules rewritten in plain English from the organisation’s Information Security Classification and Handling Guide. These rules form the foundational governance logic used throughout the SMEDG framework.

**Purpose:**  
- Defines enforceable governance requirements.  
- Drives ontology modelling, SHACL constraints, and SPARQL validation rules.  
- Forms the policy baseline for competency questions (CQ1–CQ24).

**Columns:**  
- **ID**: Policy rule identifier (P1–P48)  
- **Policy Rule**: Plain-language policy statement  


### **Online Appendix Table 2: Competency Questions (CQ1–CQ24)**
This table documents all 24 competency questions (CQs) that specify the information needs the ontology must answer. Each CQ is mapped to policy rules and ontology elements.

**Purpose:**  
- Guides ontology requirements.  
- Links each CQ to relevant policy rules and necessary ontology classes/properties.

**Columns:**  
- **CQ**: Competency question ID  
- **Competency Question**: The question the ontology must answer  
- **Mapped Policy Rules**: Policy rules informing the CQ  
- **Anchor Class**: Main ontology class involved  


### **Online Appendix Table 3: SHACL/SPARQL Validation Mapping**
This table maps each competency question to the SHACL shapes and SPARQL validation queries that operationalise it.

**Purpose:**  
- Shows how each CQ is enforced in SMEDG via SHACL constraints and SPARQL logic.  
- Documents system behaviour for compliance automation.

**Columns:**  
- **CQ#**: Competency question number  
- **SHACL Check**: Description of constraint(s) applied  
- **SPARQL Return**: What the validation query reports  


### **Online Appendix Table 4: Contextual Ontology Instances (29 Instances)**
This table contains the stable, compliant baseline entities of the organisation, such as departments, roles, labels, storage services, tenants, channels, and platforms.

**Purpose:**  
- Provides the background organisational context needed to evaluate rule compliance.  
- Supplies the ontology with core entities for reasoning.

**Columns:**  
- **Category**: Type of contextual entity  
- **Instances**: List of instances in that category  
- **Description/Role**: Purpose of each category in governance  


### **Online Appendix Table 5: Scenario-Specific Instances (35 Instances)**
This table includes deliberately non-compliant scenario instances, each reflecting a violation of one or more policy rules. These are used to test the SHACL and SPARQL rules from end to end.

**Purpose:**  
- Evaluates whether SMEDG detects policy breaches correctly.  
- Provides rich test cases covering storage, sharing, labelling, retention, classification changes, GenAI usage, USB/email rules, and destruction/archiving.

**Columns:**  
- **Asset / Data Item**: Name of the file or event  
- **Instance Name(s)**: Node(s) created in the ontology  
- **Ontology Type**: Asset, Document, DistributionEvent, etc.  
- **Addressed CQ#**: Which competency question it tests  
- **Mapped Policy Rule(s)**: Policy logic being validated
-   
- **Policy Focus** — Expected behaviour according to the guide  
