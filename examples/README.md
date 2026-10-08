# Examples

This folder provides examples demonstrating how the EMBRC conceptual provenance model can be applied in practice. We have an example experiment, producing example datasets, and have created example provenance metadata -- in TXT and JSON-LD -- following the model. For the plain text examples we have adopted the class and property names (as explained in [docs](https://github.com/vliz-be-opsci/embrc-prov-model/tree/main/docs)) and simply filled in the values, for the JSON-LD examples we have followed our suggested [RDF implementation](https://github.com/vliz-be-opsci/embrc-prov-model/tree/main/implementations/RDF). 

## The example experiment
These are the research activities that will create the four datasets: 
* Step 1 You go out on a research vessel to collect a sample of water.
* Step 2 You make measurements of temperature and salinity. 
* Step 3 You perform a pre-filtering of the water sample (using a large pore-size mesh) and split it into two subsamples. One subsample is filtered again using smaller pore-size filter membrane. The resulting filter membrane and the other water sample are placed in cold storage on-board.
* Step 4 Arriving at the marine station, the single-filtered subsample is processed through a FlowCam to image the plankton community. The FlowCam produces a set of images. These images are analysed by the species-identification software within the FlowCam to produce species names together with the image filenames. Taxonomic confirmation is done on those outputs. 
* Step 5 Meanwhile, the membrane is stored in the freezer in the lab, and after some time it is shipped to a genomics facility.
* Step 6 When the genomics facility receives the filter, it is first stored and later processed to extract the DNA. The resulting sequences are stored on their cloud to be shared with others.

Three datasets result from these activities: 1) the log sheet recording data about the sampling activity and including the measured values of temperature and salinity; 2) the images created by the FlowCam from the processed material (water sample), a file with FlowCam instrument and software settings used, a protocol document that is not provided online, and one spreadsheet with the identified and confirmed species listed, and 3) the sequences, stored on the cloud of the genomics facility. You now want to share these datasets by publishing them with different data repositories for anyone else to find, access, and use. What would the provenance metadata for these three datasets look like?

## Content: 
- **Plain text files**: Human-readable, providing a simplified overview of the dataset's provenance. [Dataset1_ProvenanceMetadata.txt](https://github.com/vliz-be-opsci/embrc-prov-model/blob/main/examples/Dataset1_ProvenanceMetadata.txt) describes the log sheet, [Dataset2_ProvenanceMetadata.txt](https://github.com/vliz-be-opsci/embrc-prov-model/blob/main/examples/Dataset2_ProvenanceMetadata.txt) the FlowCam images and species list, and [Dataset3_ProvenanceMetadata.txt](https://github.com/vliz-be-opsci/embrc-prov-model/blob/main/examples/Dataset3_ProvenanceMetadata.txt) the sequences. 
- **JSON-LD files**: RDF-formatted for machine processing, enabling semantic interoperability.  [Dataset1_ProvenanceMetadata.jsonld](https://github.com/vliz-be-opsci/embrc-prov-model/blob/main/examples/Dataset1_ProvenanceMetadata.jsonld) describes the log sheet, [Dataset2_ProvenanceMetadata.jsonld](https://github.com/vliz-be-opsci/embrc-prov-model/blob/main/examples/Dataset2_ProvenanceMetadata.jsonld) the FlowCam images and species list, and [Dataset3_ProvenanceMetadata.jsonld](https://github.com/vliz-be-opsci/embrc-prov-model/blob/main/examples/Dataset3_ProvenanceMetadatajdonld) the sequences.


