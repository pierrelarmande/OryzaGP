# OryzaGP
A dataset for Named Entity Recognition for rice gene

* Find the project page on PubAnnotation repository:
http://pubannotation.org/projects/OryzaGP
* Find the development project page http://pubannotation.org/projects/OryzaGP_2021
* Dowload the OryzaGP datatset http://pubannotation.org/projects/OryzaGP_2021/annotations.tgz

## citation
Please cite with the following reference: 
Pierre Larmande, Huy Do, Yue Wang. OryzaGP: rice gene and protein dataset for named-entity recognition. Genomics Inform. 2019;17(2):e17. DOI: https://doi.org/10.5808/GI.2019.17.2.e17

## Updating OryzaGP dataset during BLAH7

The aim of this projet is to :

* update the datasets with new pubmed entries
* process annotation on gene/protein entities

### Step 1: updating OryzaGP with new pubmed entries

* Downloaded Oryza reference dataset from Oryzabase database https://shigen.nig.ac.jp/rice/oryzabase/.
  * Oryzabase provides manually curated dataset for new rice related pubmed entries 
* A list of pubmedid have been created and uploaded on http://pubannotation.org/projects/OryzaGP_2021
* Corresponding abstracts have been retrieved

### Step 2: creating a new pub dictionnary 

* In order to create or use ER tools, we need to setup a dictionary of gene/protein entities
* a first file named pub_dictionnary.txt was created from the Oryzabase gene dataset 
  * https://shigen.nig.ac.jp/rice/oryzabase/download/gene.
  * it contains a label/gene name/symbol/synonyms [TAB] Oryzabase database URI
* a second pub_dictionnary_with_rapdb_URI.txt was created from the same dataset
  * it contains a label/gene name/symbol/synonyms [TAB] RAP-DB database URI
* a third pub_dictionnary_with_msu.txt was created from the same dataset
  * it contains a label/gene name/symbol/synonyms [TAB] MSU database URI

### Step 3: creating PubDictionary Annotators
* we created 2 annotators for each pub dictionary ( single and batch mode)
