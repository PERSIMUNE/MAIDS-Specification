# Specification for the Medical AI Datasheet (MAIDS)
A versioned specification for the Medical AI Datasheet project.

*v0.2-alpha*

MAIDS is currently being prototyped for the [Copenhagen Ultrathon on Precision Medicine](https://ultrathon.online) where you will find several examples.

This repository is intended to maintain the specification for what a MAIDS document is, what it is meant to be, and best practices. The code for implementing the specification is [maintained separately](https://github.com/PERSIMUNE-Health-Informatics/MAIDS).

MAIDS is inspired by the work of [Gebru et al., 2020, in "Datasheets for datasets"](https://arxiv.org/abs/1803.09010) and is intended to expand on it as a tool for data communication in medicine.

Please watch/star if you'd like to be notified of new developments.

# The FAIR vision of Medical AI Datasheets:

FAIR Category|FAIR Subcategory|Support|Benefit of Medical AI Datasheets
---|---|---|---
To be Findable|||
---|F1. Unique|YES|Every datasheet has a unique identifier and address. Moreover, every datasheet and every version of the datasheet is uniquely represented by a cryptographic hash.
---|F2. Rich description|YES|See Interoperable:Knowledge & Reusable below. 
---|F3. Internal refs|YES|Every internal entity has an ID. Moreover, full traceability of when and who updated an entity is tracked over the full life cycle of a MAIDS document.
---|F4. Indexed|YES|The infrastructure will provide a fully featured index with methods to search the database through a web browser or programmatically by RESTful interface.
To be Accessible|||
---|A1. Retrievable|YES|Datasheets may be cloned for those only interested in working with the data; forked for those interested in collaborating; or updated either through the web browser or programmatically by the datasheet’s owner.
---|A1.1 Open protocol|YES|All code for the infrastructure will be made fully open source.
---|A1.2 Authentication|YES|The main intent is to publish fully open and sharable MAIDS descriptions. However, we recognize data owners might prefer private datasheets during specification and/or timed releases and providing this functionality may be required to on board users more frequently and with greater trust. Moreover, authentication will be required to support collaborative features as well as key performance indicators.
---|A2. Metadata|YES|This use of the term metadata by the FAIR principles should not be confused with the MAIDS specification itself, which standardizes methods of collecting medical metadata. In this instance MAIDS supports FAIR metadata by decoupling the official specification from it’s implementation.
To be Interoperable|||
---|I1. Knowledge rep.|YES|MAIDS represents knowledge of any medical dataset in four sections: CONTEXT; PURPOSE; STATISTICS; PROVENANCE. CONTEXT links a dataset to the local environment the dataset was created in. PURPOSE describes the reason the dataset exists. STATISTICS summarizes the types and distributions of the original data. PROVENANCE tracks the history of the knowledge representation.
---|I2. Vocabularies|LOOSELY|MAIDS provides only a few strict vocabularies. This is by intent and done to ensure low barrier to access. The few strict vocabularies only exist to facilitate programmatic access, again to facilitate easy use of MAIDS. Finally, other more complex projects such as OHDSI handle vocabularies with greater precision and dexterity. Our intent with a minimal vocabulary is to promote rapid and fully open community adoption that might serve as a staging area for datasets to enter OHDSI or similar projects.
---|I3. Internal refs.|YES|see Findable.
To be Reusable|||
---|R1. Rich description|YES|All datasheets will come with full knowledge representations, the code to interact with them, and reusable environments that also ensure reproducibility. All aspects of MAIDS will be fully documented. Indeed, the guiding specification of MAIDS is decoupled from the core logic implementing it and these are again treated and documented separately from the infrastructure code base. As Github projects, all parts of the project will always be open to community feedback and collaboration.
---|R1.1 License|PLANNED|We will discuss with the steering committee, experts, and the broader community what the best open license is and whether we should allow different MAIDS documents to have different types of licenses.
---|R1.2 Provenance|YES|MAIDS documents are designed from the ground up to capture provenance and enable community attribution. Data owners will also be able to view who accessed which datasheet and how datasheets are used in other projects.
---|R1.3 Community stand.|YES|The MAIDS specification enforces a standard that must be adhered to in order for a datasheet to be certified “MAIDS”. The specification is a “living document”, continuously updated with community collaboration.

