# EML implementation

This folder contains resources related to the EML implementation of the provenance model.
[EML](https://eml.ecoinformatics.org/) is the Ecological Metadata Language that is an XML schema used by OBIS and GBIF (among others). As this schema is widely used by these biodiversity data infrastructures, and is the _ecological_ metadata language, we tried to develop an implementation of our conceptual model in EML. Unfortunately, this resulted in many gaps, which are marked in red in the diagrams. Eventually we realised that if the provenance model is to be accommodated in EML it will require expanding the schema, rather than distorting it. Last update: Oct 2026

- `./diagrams` to contain visualization of EML classes
- `./subyt-templates` to contains templates that can be used to generate EML XML conformant to the provenance model
