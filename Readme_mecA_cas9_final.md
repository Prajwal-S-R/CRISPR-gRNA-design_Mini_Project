### CRISPR Guide RNA Design

In this mini project on designing a guide RNA for CRISPR/Cas, we will know to download the gene from NCBI and load it to SnapGene viewer for gene map and sequence study. Then using CHOPCHOP we check the target sequence in our selected gene for the study and via excel sheet we filter those sequences and finally annotate that selected sequences in the SnapGene viewer by naming PAM and guide for specific Cas enzyme. 

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

 >> - Then next to the target box there is 'In' box, type your selected organism name (*Streptococcus pyogenes*). For 'Using' box click on CRISPR/Cas9, then for last box ('For') select activation.
  <img width="1465" height="702" alt="image-11" src="https://github.com/user-attachments/assets/93d45f2f-2f6c-4dbf-9acb-bf94aba0926c" />

 >> - Now select the 'Options', 
  in that select Cas9 and also check for PAM3 sequence as NGG and also the sgRNA length to 20bp, 
  apart from this leave other features as default. Finally click on Find Target Sites!
  <img width="1465" height="702" alt="image-12" src="https://github.com/user-attachments/assets/cd81e878-0dfb-4ec9-806f-4d8a0166f682" />
  <img width="803" height="890" alt="image-13" src="https://github.com/user-attachments/assets/b5b1aefd-5078-4da6-b8d3-332b1fb2f1a3" />
  After this step, leave it to process and find your target.
  <img width="1346" height="522" alt="image-14" src="https://github.com/user-attachments/assets/a3fcd2e0-16eb-4efa-8f69-f6a3fcab8073" />
 
 > Way : Browser -> CHOPCHOP -> Paste target -> Target (Paste your copied sequence) -> In -> Using -> For -> Options --> Find Target Sites!

 > ii) Loading the result table into Excel 
 >> The CHOPCHOP will gives many target sequences in the form of table having rank, genomic location, strand, GC content, efficiecny, self complementary,  mismatches (MM0, MM1, MM2, MM3) and a visual map at the top.
<img width="1886" height="872" alt="image-16" src="https://github.com/user-attachments/assets/c6ef2ad5-55af-474a-b072-e0b02e3dd402" />
 Now you have to click on dropdown named as 'Please select one' (Download results). 
  In that opt for "Results table as .tsv" , it will downloads the result.
<img width="1856" height="975" alt="image-15" src="https://github.com/user-attachments/assets/a8a65c51-cecf-4ac2-a698-c57747ca0554" />
 After downloading, right click on result file and select 'edit in notepad', copy the whole table content by pressing Ctrl+A --> Ctrl+C.
<img width="1625" height="996" alt="image-17" src="https://github.com/user-attachments/assets/8513083f-e18f-46ff-9b3d-ba8dcd576d1a" />
 Paste it into a new microsoft Excel sheet.
<img width="1236" height="777" alt="image-18" src="https://github.com/user-attachments/assets/6b35334f-c493-4ce1-bfc4-7476b2096ac8" />

 #### Step 4 : Analysing the result by filtering
 Paste the .tsv file by pressing Ctrl+V into one cell. Now click on first row and select Filter options in the 'Sort & filter' (Editing ribbon of Home tab).
<img width="1917" height="630" alt="image-20" src="https://github.com/user-attachments/assets/2ed28c6f-1a3c-4610-8ff2-8e76f229c272" />
 Observe the tiny dropdown menu after the names of first row.
 <img width="1917" height="542" alt="image-21" src="https://github.com/user-attachments/assets/a045b54e-f02e-4bda-a056-8bdf9d9ac68a" />
 Now click on the tiny dropdown, it will pop up certain tick box and there optimise the values. 
- We usually set following parameters which has already been standardized by scientist and industrial peoples.
>a) GC content = 40 - 60%
<img width="1090" height="732" alt="image-23" src="https://github.com/user-attachments/assets/bdedd53b-f229-4709-b469-b0d87a169ff1" />

 >b) Efficiency = >50 % 
<img width="1151" height="652" alt="image-24" src="https://github.com/user-attachments/assets/70351cc1-dc58-491f-b0df-6793af6f5d40" />

>c) Self-complementary = 0
<img width="1101" height="627" alt="image-25" src="https://github.com/user-attachments/assets/8e29292e-44bc-4335-b495-e835f9194fbb" />

>d) Mismatches (MM0 = 1, MM1, MM2, MM3 = 0)

After filtering above parameters, the result has only two target sequences -           TTGATTGAGCATGCAAACCCTGG and TTCAACGATTACAGAGGCAGTGG

<img width="1277" height="227" alt="image-26" src="https://github.com/user-attachments/assets/90ca0cec-faf4-46ef-b81d-4a6b9da77a20" />
Now we have to copy the target sequence and find in the SnapGene viewer for the position and orientation. 

 #### Step 5 : Higlighting the Guide 
 I have copied the first target sequence (TTGATTGAGCATGCAAACCCTGG) from the above result excel sheet. Then go to SnapGene viewer software, press Ctrl+F --> opens dialogue box in the bottom of the page.
 <img width="1707" height="947" alt="image-27" src="https://github.com/user-attachments/assets/9a56fc3e-9146-4da0-b7dd-6a5909efefd8" />

Paste it here by pressing Ctrl+V. Then press next.
<img width="1917" height="318" alt="image-28" src="https://github.com/user-attachments/assets/87b37941-6d09-46b4-abcb-88c7919de3e5" />

The software will locate your target sequence like this below as highlighted (green).
<img width="1812" height="922" alt="image-29" src="https://github.com/user-attachments/assets/dba10396-0c7f-4a00-b27f-365c2e01f306" />

Observe keenly your PAM for Cas9 (NGG) in the target. Here PAM is **'TGG'**, to visualise differentiate it, add a feature named as PAM. For this select the PAM sequence and then go to Features --> Add feature 
<img width="1740" height="977" alt="image-31" src="https://github.com/user-attachments/assets/d4db7998-e32b-415f-a8a4-d5184bb9315d" />

In feature, rename it to PAM and change the color, press ok.
<img width="1840" height="887" alt="image-32" src="https://github.com/user-attachments/assets/4a0dd592-55fd-487e-8e89-1eccbfb5a882" />
It features like this and here after designing guide, check for the homopolymers in seed region and also the GC content. 
<img width="1702" height="472" alt="image-33" src="https://github.com/user-attachments/assets/e1675b6a-cc51-48c8-9162-b39e3df20a51" />

Note: In CRISPR guide design, homopolymers (stretches of 4 or more identical consecutive bases, e.g., AAAA or TTTT) in the seed region are bad. They frequently cause off-target cutting, reduce on-target editing efficiency, and introduce synthesis or sequencing errors.

Likewise, select the remaining 20bp in target and add feature as Guide_1_Cas9.
<img width="1822" height="967" alt="image-34" src="https://github.com/user-attachments/assets/d2e4975c-adf6-494a-80ad-dd4f43c4c591" />

After adding feature, PAM and guide looks like this in the sequence map. 
<img width="1632" height="747" alt="image-35" src="https://github.com/user-attachments/assets/317742b4-dee7-45ce-b7fb-21ff6b2c94e5" />

For the second target sequence, follow the above steps (Step 5) sequentially. Doing this will leads to appear like this.
<img width="1857" height="792" alt="image-36" src="https://github.com/user-attachments/assets/e74f357b-0ed5-47ca-900a-4bc8cca9b54f" />
In the above image, I have designed two guide sequences for cas9 (Check report folder for .dna file of this). In this way one can create guide RNA for CRISPR/Cas9. Further one can check if the sequences are conserved or not by doing BLAST of the target sequence and finalise using tools like jalview, geneious prime.

