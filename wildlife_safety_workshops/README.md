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

You're a biologist with the FDA. A shipment of mangos from Spain was received in the Baltimore shipment yard. Upon inspection of one of the crates, you see a few mangos have small dots on them that could be insect eggs. Before allowing the mangos to pass through the border and go into supermarkets, you want to be sure that those black dots aren't harmful. You don't want to introduce an invasive species or toxic organism into the US that could affect the mangos grown in Florida or California. You take the mangos with the small black dots on them back to the lab, extract DNA from the black dots, and [sequence](wildlife_safety_workshops_data/sample_1.fasta) the CO1 gene. There are now 50,000 mangos sitting in a warehouse. Depending on your results, it is up to you to decide if the mangos will be allowed into the country.

#### Goals: 
1. Understand the format of a fasta file.
2. Uploading to BLAST and performing a search.
3. Understanding the BLAST results.
4. Reading an NCBI accession.
5. Determine the results.

<!--Results: fruit fly-->
<br><br>

## Bio-terrorism Scenario 

Three letters are delivered to the Pentagon, White House, and Capital building. An assistant at each government building opens thier respective envelope to find a letter and white powdery substance inside it. As an FBI investigative agent, you are called in to investigate these suspecious letters and unknown white substance. Each building that received a letter is quarantined until the genetic results are obtained. Each unknown white substance was amplified with primers useful for identifying most plants, animals, and bacteria, and sequences [1](wildlife_safety_workshops_data/sample_2a.fasta), [2](wildlife_safety_workshops_data/sample_2b.fasta), and [3](wildlife_safety_workshops_data/sample_2c.fasta) were obtained. Upon receiving the results, you need to decide if a building can be released or if the building needs to remain under quarantine, and the people inside need to receive medical attention.


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

An individual is walking through airport customs security and pulled aside for a suspicious item in their bag. As a U.S. Customs and Border Agriculture Specialist, you are called over to help with the inspection. A small, heavy engraved object is pulled out from within several pairs of socks. From your years of experience you immediately suspect this as ivory. However, you are unsure if this is ivory from an elephant or walrus tusk, a rhino horn, or a different animal. You send off the sample to be confirmed that it is ivory and for genetic testing to find out the species it belongs to. You receive documentation that it is a positive result for ivory and a [CO1 sequence](wildlife_safety_workshops_data/sample_3.fasta). Your job is to idenity which species this piece of ivory came form. 

### Goals:
1. Perform a BLAST search and identify the species.

<br>

### Poaching Analysis

You now know that the piece of ivory belongs to a white rhinoceros *Ceratotherium simum*. Because white rhinos are endangered, your suspicions rise. Is this a case of poaching? Was the rhino killed? Is the rhino from a zoo or a wildlife sanctuary? The two most common types of rhinos that are poached are white rhinoceroses and black rhinoceroses. You compile a list of [sequences](wildlife_safety_workshops_data/part_3_sequences.fasta) from known white and black rhinoceroses. You also include two sequences from horses as outgroups, because horses are most closely related to rhinos. Using your list of sequences, you will perform a [mulitple alignment search](wildlife_safety_workshops_data/part_3_alignment.phy). All the sequences you are using are assumed to have an evolutionary relationship. This means that the sequences (rhinos and horses) descended from a common ancestor. Performing a multiple alignment search allows sequence homology to be inferred. Followed by [phylogenetic analysis](wildlife_safety_workshops_data/part_3_tree.tre), the evolutionary origins of the sequences can be assessed.

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
