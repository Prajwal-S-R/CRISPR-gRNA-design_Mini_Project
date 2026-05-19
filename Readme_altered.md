[Readme_gRNA_Cas9.md](https://github.com/user-attachments/files/27964083/Readme_gRNA_Cas9.md)
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
  ![alt text](image-11.png)
 >> - Now select the 'Options', 
  in that select Cas9 and also check for PAM3' sequence as NGG or else and also the gRNA length of 20bp, 
  apart from this leave other features as default. Finally click on Find Target Sites!
  ![alt text](image-12.png)
  ![alt text](image-13.png)
  After this step, leave it to process and find your target.
  ![alt text](image-14.png)
 
 > Way : Browser -> CHOPCHOP -> Paste target -> Target (Paste your copied sequence) -> In -> Using -> For -> Options --> Find Target Sites!

 > ii) Loading the result table into Excel 
 >> The CHOPCHOP will gives many target sequences in the form of table having rank, genomic location, strand, GC content, efficiecny, self complementary,  mismatches (MM0, MM1, MM2, MM3) and a visual map at the top.
 ![alt text](image-16.png)
 Now you have to click on dropdown named as 'Please select one' (Download results). 
  In that opt for "Results table as .tsv" , it will downloads the result.
 ![alt text](image-15.png)
 After downloading, right click on result file and select 'edit in notepad', copy the whole table content by pressing Ctrl+A --> Ctrl+C.
 ![Notepad view](image-17.png)
 Paste it into a new microsoft Excel sheet.
 ![alt text](image-18.png)

 #### Step 4 : Analysing the result by filtering
 Paste the .tsv file by pressing Ctrl+V into one cell. Now click on first row and select Filter options in the 'Sort & filter' (Editing ribbon of Home tab).
 ![alt text](image-20.png)
 Observe the tiny dropdown menu after the names of first row.
 ![alt text](image-21.png)

 Now click on the tiny dropdown, it will pop up certain tick box and there optimise the values. 
- We usually set following parameters which has already been standardized by scientist and industrial peoples.
>a) GC content = 40 - 60%
![alt text](image-23.png)

 >b) Efficiency = >50 % 
 ![alt text](image-24.png)


>c) Self-complementary = 0
![alt text](image-25.png)

>d) Mismatches (MM0 = 1, MM1, MM2, MM3 = 0)

After filtering above parameters, the result has only two target sequences -           TTGATTGAGCATGCAAACCCTGG and TTCAACGATTACAGAGGCAGTGG

![alt text](image-26.png)
Now we have to copy the target sequence and find in the SnapGene viewer for the position and orientation. 

 #### Step 5 : Higlighting the Guide 
 I have copied the first target sequence (TTGATTGAGCATGCAAACCCTGG) from the above result excel sheet. Then go to SnapGene viewer software, press Ctrl+F --> opens dialogue box in the bottom of the page.
 ![alt text](image-27.png)

Paste it here by pressing Ctrl+V. Then press next.
![alt text](image-28.png)

The software will locate your target sequence like this below as highlighted (green).
![alt text](image-29.png)

Observe keenly your PAM for Cas9 (NGG) in the target. Here PAM is 'TGG', to visualise differentiate it, add a feature named as PAM. For this select the PAM sequence and then go to Features --> Add feature 
![alt text](image-31.png)

In feature, rename it to PAM and change the color, press ok.
![alt text](image-32.png)
It features like this
![alt text](image-33.png)

Likewise, select the remaining 20bp in target and add feature as Guide_1_Cas9.
![alt text](image-34.png)

After adding feature, PAM and guide looks like this in the sequence map. 
![alt text](image-35.png)

For the second target sequence, follow the above steps (Step 5) sequentially. Doing this will leads to appear like this.
![alt text](image-36.png)
In the above image, I have dsigned two guide sequences for cas9. In this way one can create guide RNA for CRISPR/Cas9. 

