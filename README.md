# Whodunit? Forensics with DNA & Bioinformatics Workshop

The workshop will analyze DNA sequence data to identify the gene(s) involved and identify the context of the samples by linking to PubMed records. You will analyze DNA sequence data using local alignment, global alignment, multiple sequence alignment tools and then use your multiple sequence alignment to estimation evolutionary (phylogenetic) relationships amongst the sequences.  With the phylogeny in hand, you will then solve the forensic mystery and decide if the accused is innocent or guilty of an alleged crime. You will gain experience using a diversity of open-access tools that are all available online. 
## Goals:
1. Perform BLAST search to identify sequence region (local alignment)
2. Link to study system via PubMed link on GenBank entry
3. Conduct a multiple sequence alignment (global alignment) using MAFFT
4. Estimate a Neighbor-Joining phylogeny
5. Interpret your phylogenetic estimate relative to the forensics case

### Part 0 - Looking at Sequence Data
1.	Take a look at the [sequence data](https://github.com/hdehart/HIV_Workshop/blob/master/data_subset.fas). This dataset contains multiple sequences in [FASTA](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=BlastHelp) format. This is a standard format for DNA sequence data developed by [David Lipman](http://www.people.virginia.edu/~wrp/) and [William Pearson](https://www.amia.org/about-amia/leadership/acmi-fellow/david-j-lipman-md-facmi). Copy the first nucleotide sequence. Each sequence starts with a title to separate it from others in the same file:

\>**AY156858.1**\_*V01*

\>**Accession number**\_*Sample name*

An [accession number](https://www.ncbi.nlm.nih.gov/genbank/sequenceids/) is a unique ID assigned to sequences uploaded to the [GenBank database](https://www.ncbi.nlm.nih.gov/genbank/). The sample names include information about who the sample came from:

1. Go to [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi) What option(s) might you choose given your data?  Why?
2. Run a BLAST - What are the options? What do these mean?  What are your parameter values?  How do those impact your search?
3. Explore the results of the BLAST search. Click on the accession number of the top hit. What do you think this sequence is? Who did it come from? 

### Part 1 - Creating a Multiple Sequence Alignment (MSA)
You now know that you have sequences from multiple samples and different sources. You need to compare the similarities and differences between the sequences, but how do we do that? 


![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/grapefruit.png) ![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/orange.png)

*[source](https://commons.wikimedia.org/wiki/User:Evan-Amos/Food)*

Look at these 2D pictures of a grapefruit and an orange. Are there differences you can see? Are there differences you can’t see in this format? Would looking at the real fruits in person better inform your ideas about similarities and differences?

This is why we create multiple sequence alignments! Lining up the sequences helps us determine the similarities and differences among sequences. We do this quickly by using alignment software.

1.	Go to the [MAFFT alignment online software](https://mafft.cbrc.jp/alignment/server/) and explore some ways to create a multiple sequence alignment. If you change default settings, compare with others and see if and what parameters make a big difference in the alignments you create.
2.	Look at the different ways the sequences were aligned. At the bottom of each alignment, there are symbols to indicate shared and different amino acid bases.

|Symbol|Meaning|
:-------:|-------|
|\* | All the sequences are the same
|\. | There are differences between some or all of the sequences

3.	Can you spot some differences between the different sample sequences? Are there shared similarities between P samples and V samples? What about LA samples?

### Part 2 - Estimating Phylogenetic Relationships and Trees

Now that the sequences are [aligned](https://github.com/hdehart/HIV_Workshop/blob/master/data_aligned.fas) and we can see all the similarities and differences, we need to determine which ones are more and less alike. How can we do that? Let's think back to the fruits...

![alt text](https://github.com/hdehart/HIV_Workshop/blob/master/fruit_tree.PNG)

Think about some charactersitics that are shared among different types of fruits. All fruits are more similar to each other than they are to a vegetable, like an onion. Within fruits however, some are more closely related because of shared characteristics. For example, the orange and grapefruit are more similar to each other than either is to an apple, because they are citrus fruits. Peaches and cherries are more similar to each other than either is to the apple, because they only have a single pit. 

Let’s think about our HIV sequences the same way by estimating a phylogenetic tree. 

1.	Create a hypothesis. If some sequences are more similar to each other, what do you think the tree will look like?
2.	Go back to the alignment you created and create a phylogenetic tree out of the alignment you created. What do you think each of the parameters adjusts? Do you think adjusting these parameters will greatly affect your results?
6.	Look at the tree you made. Do you see any groupings of sequences? Which sequence groups do you think are more or less closely related? Why? 

### Part 3 - Solve a Crime...

You are a researcher in a forensics laboratory. You are contacted by a lawyer representing a victim who accuses her physician of intentionally infecting her with the Human Immunodeficiency Virus (HIV) after their romantic relationship ended. After receiving a vitamin B-12 injection from this doctor, the victim tested positive for HIV. The lawyer alleges that the shot contained infected blood from other HIV positive patients under the doctor’s care. Using HIV sequences from victim, patients of the doctor, and other people in the area, it is up to you to determine if the victim could have contracted HIV from her doctor’s shot or some other source.

1. Create a new hypothesis. If the doctor **DID** infect the victim, do you think her HIV sequences will be more or less similar to other HIV positive patients than they would be to random HIV positive individuals? Why?
2.	Go back to your original BLAST results. Click on accession number AY156858.1.  Hit the second [PUBMED](https://www.ncbi.nlm.nih.gov/pubmed/) link (to the PNAS paper).  Where does this take you? 
3. Read the abstract, click on the [DOI](https://www.doi.org/). How did your analysis compare to the published study? Guilty or Not Guilty?

More information on this case:

[ABC News](https://abcnews.go.com/Technology/story?id=97856&page=1)

[The Advocate](https://www.theadvocate.com/acadiana/news/article_4f2c8962-fd3c-5fa7-87cf-048188f626e3.html)

# Bioinformatic Workshop 
## Wildlife and Safety Bioinformatic Workshop


## Tools
#### These will be the tools we will be using:

* [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastSearch)
* [PHYLO "Interactive alignment game"](http://phylo.cs.mcgill.ca "Interactive alignment game")
* [Evolution tree game](http://tidal.northwestern.edu/blog/bat/#level1)
* [CIPRES](http://www.phylo.org)
* [Interactive Tree of Life](https://itol.embl.de)
<!--* [Phylotastic!](http://phylo.cs.nmsu.edu:3000)-->
<br><br>

## Imported Goods Scenario

You're a biologist with the FDA. A shipment of mangos from Spain was received in the Baltimore shipment yard. Upon inspection of one of the crates, you see a few mangos have small dots on them that could be insect eggs. Before allowing the mangos to pass through the border and go into supermarkets, you want to be sure that those black dots aren't harmful. You don't want to introduce an invasive species or toxic organism into the US that could affect the mangos grown in Florida or California. You take the mangos with the small black dots on them back to the lab, extract DNA from the black dots, and [sequence](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/sample_1.fasta) the CO1 gene. There are now 50,000 mangos sitting in a warehouse. Depending on your results, it is up to you to decide if the mangos will be allowed into the country.

#### Goals: 
1. Understand the format of a fasta file.
2. Uploading to BLAST and performing a search.
3. Understanding the BLAST results.
4. Reading an NCBI accession.
5. Determine the results.

<!--Results: fruit fly-->
<br><br>

## Bio-terrorism Scenario 

Three letters are delivered to the Pentagon, White House, and Capital building. An assistant at each government building opens thier respective envelope to find a letter and white powdery substance inside it. As an FBI investigative agent, you are called in to investigate these suspecious letters and unknown white substance. Each building that received a letter is quarantined until the genetic results are obtained. Each unknown white substance was amplified with primers useful for identifying most plants, animals, and bacteria, and sequences [1](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/sample_2a.fasta), [2](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/sample_2b.fasta), and [3](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/sample_2c.fasta) were obtained. Upon receiving the results, you need to decide if a building can be released or if the building needs to remain under quarantine, and the people inside need to receive medical attention.


#### Goals: 
1. Perform multiple BLAST searches.
2. Identify species.
3. Determine if the species is harmful or harmless.

<br>

*Additional information about the anthrax case*
* https://www.fbi.gov/history/famous-cases/amerithrax-or-anthrax-investigation

<!--Results: wheat flour, rice flour, Bacillus anthracis 16s partial sequence-->
<br><br>

## Poaching Scenario
### Smuggling Identification

An individual is walking through airport customs security and pulled aside for a suspicious item in their bag. As a U.S. Customs and Border Agriculture Specialist, you are called over to help with the inspection. A small, heavy engraved object is pulled out from within several pairs of socks. From your years of experience you immediately suspect this as ivory. However, you are unsure if this is ivory from an elephant or walrus tusk, a rhino horn, or a different animal. You send off the sample to be confirmed that it is ivory and for genetic testing to find out the species it belongs to. You receive documentation that it is a positive result for ivory and a [CO1 sequence](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/sample_3.fasta). Your job is to idenity which species this piece of ivory came form. 

### Goals:
1. Perform a BLAST search and identify the species.

<br>

### Poaching Analysis

You now know that the piece of ivory belongs to a white rhinoceros *Ceratotherium simum*. Because white rhinos are endangered, your suspicions rise. Is this a case of poaching? Was the rhino killed? Is the rhino from a zoo or a wildlife sanctuary? The two most common types of rhinos that are poached are white rhinoceroses and black rhinoceroses. You compile a list of [sequences](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/part_3_sequences.fasta) from known white and black rhinoceroses. You also include two sequences from horses as outgroups, because horses are most closely related to rhinos. Using your list of sequences, you will perform a [mulitple alignment search](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/part_3_alignment.phy). All the sequences you are using are assumed to have an evolutionary relationship. This means that the sequences (rhinos and horses) descended from a common ancestor. Performing a multiple alignment search allows sequence homology to be inferred. Followed by [phylogenetic analysis](https://github.com/gwcbi/Bioinformatic_workshops/blob/master/part_3_tree.tre), the evolutionary origins of the sequences can be assessed.

### Goals:
1. Make an account on CIPRES
2. Perform an alignment with MUSCLE on CIPRES.
3. Preform a RAXML phylogenetic tree search with CIPRES.
4. Upload the tree into iTOL.
5. View relationships of rhinos and determine where your unknown rhino sample belongs.

<!--Results: sample belongs to the French Zoo population-->

<br>

*Additional information about rhino poaching*
* http://www.npr.org/2017/03/11/519807756/poachers-kill-white-rhino-in-french-zoo-saw-off-horn
* http://www.bbc.com/news/world-asia-39268084
