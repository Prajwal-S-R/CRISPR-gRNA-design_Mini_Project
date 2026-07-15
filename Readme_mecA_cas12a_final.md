## CRISPR guide RNA design for Cas12a
Cas12a (formerly Cpf1) and Cas12b (formerly C2c1) are RNA-guided endonucleases in the Type V CRISPR-Cas system. Both serve as highly specific molecular scissors that bind to Thymine-rich (T-rich) PAM sites instead of the G-rich PAMs targeted by Cas9, and both cleave double-stranded DNA to create staggered, 4-5 base pair overhangs.
In this section, we will see how to design ude for Cas12a which is the diagnostically important like that of Cas12b and both are extensively used as diagnostic tool in India for CRISPR/cas system for therapy in healthcare.

### Acknowledgements

 - [NCBI ](https://www.ncbi.nlm.nih.gov/)
 - [SnapGene Viewer](https://snapgene-viewer.software.informer.com/4.1/)
 - [CHOPCHOP](https://chopchop.cbu.uib.no/)


### Documentation

This section contains procedural step one should follow to design gRNA.

#### Step 1 : Selecting the suitable gene from NCBI database
- I have chosen the AMR gene mecA which is a bacterial gene that confers resistance to methicillin, penicillin, and other beta-lactam antibiotics by encoding the protein PBP2a (penicillin-binding protein 2A) which is responsible for the methicillin resistance. 
- I selected [mecA](https://www.ncbi.nlm.nih.gov/gene/69900206) from *Streptococcus pyogenes* with Gene ID: 69900206
- Download the Gene sequence in FASTA format by selecting the menu download datasets and 
  mark the Gene sequence (FASTA), then download the file named mecA_datasets.zip.
 <img width="1842" height="927" alt="1" src="https://github.com/user-attachments/assets/c8d0eee5-853c-4e65-b3cc-61ad27e8a971" />

- Extract the zip file, open ncbi_dataset --> data and there rename the gene as mecA_gene.
  <img width="1230" height="362" alt="image" src="https://github.com/user-attachments/assets/67cad138-9bfe-43bb-b948-0a2834b5fbca" />

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
Below is the steps followed for the guide RNA for Cas12a enzyme.

> i) Loading the sequence to CHOPCHOP interface
>> - After opening the CHOPCHOP, click on the menu 'paste target' which will changes to Gene target. 
  Now paste your copied sequence (from snapgene) into the 'target' box.
  <img width="1476" height="632" alt="image-10" src="https://github.com/user-attachments/assets/0007a3bf-bcb3-413e-9d5f-3f44b5364b03" />

 >> - Then next to the target box there is 'In' box, type your selected organism name *Streptococcus pyogenes* . For 'Using' box click on CRISPR/Cpf1 or Cas12 or CasX, then for last box ('For') select knock-out.
  <img width="1692" height="727" alt="image" src="https://github.com/user-attachments/assets/8cf21b7d-7d3c-4b6e-a053-68751996c4c4" />

 >> - Now select the 'Options', 
  in that select Cpf1 and also check for 'PAM' sequence as TTTN and also the sgRNA length to 20bp, 
  apart from this leave other features as default. Finally click on Find Target Sites!
  <img width="1538" height="912" alt="image" src="https://github.com/user-attachments/assets/4e6188e7-59dd-443c-a3b9-a547fc7a719e" />
  After this step, leave it to process and find your target.
  <img width="1346" height="522" alt="image-14" src="https://github.com/user-attachments/assets/a3fcd2e0-16eb-4efa-8f69-f6a3fcab8073" />

 > ii) Loading the result table into Excel 
 >> The CHOPCHOP will gives many target sequences in the form of table having rank, genomic location, strand, GC content, efficiecny, self complementary,  mismatches (MM0, MM1, MM2, MM3) and a visual map at the top. Now you have to click on dropdown named as 'Please select one' (Download results). In that opt for "Results table as .tsv" , it will downloads the result. After downloading, right click on result file and select 'edit in notepad', copy the whole table content by pressing Ctrl+A --> Ctrl+C. Paste it into a new microsoft Excel sheet.
<img width="1236" height="777" alt="image-18" src="https://github.com/user-attachments/assets/6b35334f-c493-4ce1-bfc4-7476b2096ac8" />

#### Step 4 : Analysing the result by filtering
 Paste the .tsv file by pressing Ctrl+V into one cell. Now click on first row and select Filter options in the 'Sort & filter' (Editing ribbon of Home tab).
<img width="1917" height="630" alt="image-20" src="https://github.com/user-attachments/assets/2ed28c6f-1a3c-4610-8ff2-8e76f229c272" />
 Observe the tiny dropdown menu after the names of first row.
 <img width="1917" height="542" alt="image-21" src="https://github.com/user-attachments/assets/a045b54e-f02e-4bda-a056-8bdf9d9ac68a" />
 Now click on the tiny dropdown, it will pop up certain tick box and there optimise the values. 
- We usually set following parameters which has already been standardized by scientist and industrial peoples.
>a) GC content = 40 - 60%
>b) Efficiency = >50 % 
>c) Self-complementary = 0
>d) Mismatches (MM0 = 1, MM1, MM2, MM3 = 0)
<img width="1485" height="442" alt="image" src="https://github.com/user-attachments/assets/57c818f2-8fb0-4dd9-bea4-4457231c40f2" />

#### Step 5 : Higlighting the Guide 
Copy the individual sequence from the above result excel sheet (Here only check for homopolymers in seed region) and select it. Then go to SnapGene viewer software, press Ctrl+F --> opens dialogue box in the bottom of the page.
Paste it here by pressing Ctrl+V. Then press next. The software will locate your target sequence like this below as highlighted (green).
<img width="1780" height="850" alt="image" src="https://github.com/user-attachments/assets/6cf238fe-27b2-465e-8fc7-8dff97f136a6" />

Observe keenly your PAM for Cas12a (5′-TTTN-3′) in the target. Here PAM is **'TTTG'**, to visualise differentiate it, add a feature named as PAM. For this select the PAM sequence and then go to Features --> Add feature --> rename it to PAM and change the color, press ok. Likewise also add feature for guide and finally it appears like this.
<img width="1742" height="742" alt="image" src="https://github.com/user-attachments/assets/fb6255b5-5059-4bed-bf01-3b3d44bbb8d2" />

For the remaining target sequence, follow the above steps (Step 5) sequentially. Doing this will leads to appear like the below shown. 
<img width="1860" height="794" alt="image" src="https://github.com/user-attachments/assets/a1d803e8-2149-42c0-8376-cd2f23b50e58" />
In this guide design, I have chosen 3 sequences as guide among eight target sequences. In this I selected the guide based on the lesser homopolymer sequences. 
In the above image, I have designed three guide sequences for cas12a (Check report folder for .dna file of this). In this way one can create guide RNA for CRISPR/Cas12a. Further one can check if the sequences are conserved or not by doing BLAST of the target sequence and finalise using tools like jalview, geneious prime.


