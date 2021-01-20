# OryzaGP
A dataset for Named Entity Recognition for rice gene

* Find the project page on PubAnnotation repository:
http://pubannotation.org/projects/OryzaGP
* Find the development project page http://pubannotation.org/projects/OryzaGP_2021

## Updating OryzaGP dataset during BLAH7

The aim of this projet is to :

- update the datasets with new pubmed entries
- process annotation on gene/protein entities

### Step one: updating OryzaGP with new pubmed entries

- Downloaded Oryza reference dataset from Oryzabase database https://shigen.nig.ac.jp/rice/oryzabase/.
Oryzabase provides manually curated dataset for new rice related pubmed entries 
- A list of pubmedid have been created and uploaded on http://pubannotation.org/projects/OryzaGP_2021
- Corresponding abstracts have been retrieved

### Step two: creating a new pub dictionnary 

- In order to create or use ER tools, we need to setup a dictionary of gene/protein entities
- a first file named pub_dictionnary.txt was created from the Oryzabase gene dataset https://shigen.nig.ac.jp/rice/oryzabase/download/gene.
-- it contains a label/gene name/symbol/synonysm [TAB] Oryzabase database URI
