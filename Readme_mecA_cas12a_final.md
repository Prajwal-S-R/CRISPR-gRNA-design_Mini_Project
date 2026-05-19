## CRISPR guide RNA design for Cas12a
Cas12a (formerly Cpf1) and Cas12b (formerly C2c1) are RNA-guided endonucleases in the Type V CRISPR-Cas system. Both serve as highly specific molecular scissors that bind to Thymine-rich (T-rich) PAM sites instead of the G-rich PAMs targeted by Cas9, and both cleave double-stranded DNA to create staggered, 4-5 base pair overhangs.
In this section, we will see how to design guide for Cas12a which is diagnostically important like that of Cas12b and both are extensively used as diagnostic tool in India for CRISPR/cas system for therapy in healthcare.

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
  <img width="1230" height="362" alt="image" src="https://github.com/user-attachments/assets/67cad138-9bfe-43bb-b948-0a2834b5

#### Step 2 : Loading the mecA_gene to preinstalled SnapGene Viewer software
- In 2 ways we can load the mecA_gene file into snapgene viewer.
>i) By double clicking on the mecA_gene file, which will redirects to snapgene viewer.

>ii) By right click on this file, select the option 'Edit in Notepad'. There select the gene sequence by dragging your mouse.
<img width="1025" height="382" alt="image-2" src="https://github.com/user-attachments/assets/36a6637f-3816-4890-b87d-cb7b66095ac4" />

 - After copying the sequences, open SnapGene viewer software and click File --> Create New DNA file --> opens a dialogue box
<img width="865" height="747" alt="image-3" src="https://github.com/user-attachments/assets/e2126bc2-0341-4245-99cf-340fc98aecca" /> 

 - Paste the sequence in this box and press ok.
<img width="866" height="641" alt="image-5" src="https://github.com/user-attachments/assets/da9dd10a-357d-4f95-b346-ed9fcc6ee79a" />

- It generates a map of mecA gene
<img width="1915" height="490" alt="image-6" src="https://github.com/user-attachments/assets/f60fa953-4f44-4ab6-a39a-83c6466de2c2" />

- In the bottom there are many options like map, sequence, enzyme and so on. In that opt for 'Sequence'.
<img width="1912" height="1077" alt="image-7" src="https://github.com/user-attachments/assets/21c396f1-c738-41ff-9811-d3cc6983b7d9" />
  
- Select the complete sequence and copy it (Ctrl+C).
<img width="1812" height="947" alt="image-8" src="https://github.com/user-attachments/assets/36b1827a-2d81-4fbc-bb65-ec9c3a41e648" />

#### Step 3 : Open CHOPCHOP in browser
<img width="1467" height="712" alt="image-9" src="https://github.com/user-attachments/assets/91ad08f5-2ded-4131-bf6b-775c45132713" />
Below is the steps followed for the guide RNA for Cas9 enzyme.
> i) Loading the sequence to CHOPCHOP interface
>> - After opening the CHOPCHOP, click on the menu 'paste target' which will changes to Gene target. 
  Now paste your copied sequence (from snapgene) into the 'target' box.
  <img width="1476" height="632" alt="image-10" src="https://github.com/user-attachments/assets/0007a3bf-bcb3-413e-9d5f-3f44b5364b03" />
 >> - Then next to the target box there is 'In' box, type your selected organism name ( *Streptococcus pyogenes* ). For 'Using' box click on CRISPR/Cpf1 or Cas12 or CasX, then for last box ('For') select knock-out.
  <img width="1692" height="727" alt="image" src="https://github.com/user-attachments/assets/8cf21b7d-7d3c-4b6e-a053-68751996c4c4" />

 >> - Now select the 'Options', 
  in that select Cpf1 and also check for 'PAM3' sequence as TTTN and also the sgRNA length to 20bp, 
  apart from this leave other features as default. Finally click on Find Target Sites!
  <img width="1538" height="912" alt="image" src="https://github.com/user-attachments/assets/4e6188e7-59dd-443c-a3b9-a547fc7a719e" />

  After this step, leave it to process and find your target.
  <img width="1346" height="522" alt="image-14" src="https://github.com/user-attachments/assets/a3fcd2e0-16eb-4efa-8f69-f6a3fcab8073" />
 
