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

 Note : SnapGene viewer or Benchling can be used for our work.

 #### Step 2 : Loading the mecA_gene to preinstalled SnapGene Viewer software
- In 2 ways we can load the mecA_gene file into snapgene viewer.
>i) By double clicking on the mecA_gene file, which will redirects to snapgene viewer.

>ii) By right click on this file, select the option 'Edit in Notepad'. There select the gene sequence by dragging your mouse.
<img width="1025" height="382" alt="image-2" src="https://github.com/user-attachments/assets/36a6637f-3816-4890-b87d-cb7b66095ac4" />

 - After copying the sequences, open SnapGene viewer software and click File --> Create New DNA file --> opens a dialogue box
<img width="865" height="747" alt="image-3" src="https://github.com/user-attachments/assets/e2126bc2-0341-4245-99cf-340fc98aecca" /> 

 - Paste the sequence in this box and press ok. It generates a map of mecA gene
<img width="1915" height="490" alt="image-6" src="https://github.com/user-attachments/assets/f60fa953-4f44-4ab6-a39a-83c6466de2c2" />

- In the bottom there are many options like map, sequence, enzyme and so on. In that opt for 'Sequence'.
<img width="1912" height="1077" alt="image-7" src="https://github.com/user-attachments/assets/21c396f1-c738-41ff-9811-d3cc6983b7d9" />
  
- Select the complete sequence and copy it (Ctrl+C).
<img width="1812" height="947" alt="image-8" src="https://github.com/user-attachments/assets/36b1827a-2d81-4fbc-bb65-ec9c3a41e648" />

- Extract the zip file, open ncbi_dataset --> data and there rename the gene as mecA_gene.
  
