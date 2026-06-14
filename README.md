### CRISPR Guide RNA Design

In this mini project on designing a guide RNA for CRISPR/Cas, we will know to download the gene from NCBI and load it to SnapGene viewer for gene map and sequence study. Then using CHOPCHOP we check the target sequence in our selected gene for the study and via excel sheet we filter those sequences and finally annotate that selected sequences in SnapGene viewer by naming PAM and guide for specific Cas enzyme. 

### Acknowledgements

 - [NCBI ](https://www.ncbi.nlm.nih.gov/)
 - [SnapGene Viewer](https://snapgene-viewer.software.informer.com/4.1/)
 - [CHOPCHOP](https://chopchop.cbu.uib.no/)


### Documentation

This section contains the procedural step one should follow to design gRNA.

#### Step 1 : Selecting the suitable gene from NCBI database
- I have chosen the AMR gene mecA which is a bacterial gene that confers resistance to methicillin, penicillin, and other beta-lactam antibiotics by encoding the protein PBP2a (penicillin-binding protein 2A) which is responsible for the methicillin resistance. 
- I selected [mecA](https://www.ncbi.nlm.nih.gov/gene/69900206) from *Streptococcus pyogenes* with Gene ID: 69900206
- Download the Gene sequence in FASTA format by selecting the menu download datasets and 
  mark the Gene sequence (FASTA), then download the file named mecA_datasets.zip.
 <img width="1842" height="927" alt="1" src="https://github.com/user-attachments/assets/c8d0eee5-853c-4e65-b3cc-61ad27e8a971" />

- Extract the zip file, open ncbi_dataset --> data and there rename the gene as mecA_gene.
  <img width="1230" height="362" alt="image" src="https://github.com/user-attachments/assets/67cad138-9bfe-43bb-b948-0a2834b5fbca" />
