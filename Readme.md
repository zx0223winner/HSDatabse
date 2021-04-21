### 1. [HSDatabase](http://hsdfinder.com/database/)
-------------------------
HSDatabase is a database of categorizing these highly similar duplicate genes (HSDs) in eukaryotes, which documented total of XX HSDs in XX plants and XX animals. There are many features in HSDatabase including, but not limited to the information of HSDs number, gene copy number and gene copy length. The protein function domains and pathway of HSDs are also collected from database of KEGG and InterProScan. What’s more, a BLAST search option is provided for users to conveniently explore potential homologous sequences of interest. The HSDatabase aims to become a useful platform for the prediction and comparative analysis of HSDs in the eukaryotic genomes of different survival environments, which might deepen our insights into the gene duplication mechanisms driving the genome adaptation.

1. The software implementation is written in Python 3 using the following custom scripts and platforms: HSDFinder.py, operation.py and pfam.py;
2. Enabling the duplicates to be filtered and annotated from BLASTP results and protein signature databases (e.g., Pfam); 
3. HSD_to_KEGG.py enabling the duplicates to be categorized under KEGG pathway functional categories; 
4. Django (3.1.5) is the Python-based web platforms to maintain the web server; pandas (1.2.2) is software library to manipulate the data.

* django framework
  * front-end: HTML,CSS,Javascript
  * back-end: python

* SQLite database
* Amazon web server (Amazon lightsail)

### 2.Common questions (FAQ):
-------------------------
*What is the database content and web interface?*
The predicted HSDs will be manually curated before submitting to the HSDatabase (Figure 1A). We filtered possible false positive HSDs with unfit gene copy length and add novel HSDs if necessary, especially, for those satisfy the criteria of near-identical protein lengths (within 10 amino acids and >80% pairwise identities). HSDatabase is built using a relational database (MySQL) allowing rapid retrieval of data and making resource easily maintainable. One entry corresponds to one eukaryote genome. The genomes can be browsed via the categories of plant and animal or the phylogeny for specific genome target (Figure 1B). The genome entry is then split into many subcategories of HSDs entries. The database access is via a web interface based on python script and provides various ways to search for HSDs entries, such as organism’s name, HSDs accession number, and gene copy name, etc (Figure 1C). HSDatabase can allow users to conveniently BLAST a query to find a homologous match (Figure 1D). HSDatabase will be updated timely and the latest version is HSDatabase v1.5, in which total of XX HSDs in XX plant genomes and XX animal genomes are identified.

### 3. Reference
X. Zhang, Yining. Hu, D. Smith (2020). HSDatabase - a database of highly similar duplicate genes in eukaryotic genomes, doi: XX.XX

### 4. Contact
For comments and questions, send a message to Xi Zhang (xzha25@uwo.ca).
Usage of this site follows AWS’s Privacy Policy. In accordance with that policy, we use Matomo to collect anonymised data on visits to, downloads from, and searches of this site.
