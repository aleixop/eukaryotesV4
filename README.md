# *eukaryotesV4* database

[![DOI](https://zenodo.org/badge/198411321.svg)](https://zenodo.org/badge/latestdoi/198411321)

*eukaryotesV4* is a curated database of V4 region of 18S rDNA. It was built to extract and taxonomically classify short metagenomic reads (mTags).  

You can download it in [fasta](db/eukaryotesV4_v8.fasta) format or [.txt file](db/eukaryotesV4_tax_v8.txt) with additional information.
A version with headers formatted to work with `dada2` is also available [here](db/eukaryotesV4_v8_dada2.fasta).

## Citation

Obiol, A., Giner, C.R., Sánchez, P., Duarte, C.M., Acinas, S.G. and Massana, R. [A metagenomic assessment of microbial eukaryotic diversity in the global ocean](https://doi.org/10.1111/1755-0998.13147). *Mol Ecol Resour*. 2020; 20: 718– 731. doi: 10.1111/1755-0998.13147

## Overview of the database

Here is a summary table with the taxonomic groups contained in *eukaryotesV4* database.

|Group                  |Supergroup     | OTU<sub>97</sub> sequences| Median length (bp)|
|:----------------------|:--------------|--------------------------:|------------------:|
|Apicomplexa            |Alveolata      |                        598|                369|
|Ciliophora             |Alveolata      |                       1975|                369|
|Colpodellida           |Alveolata      |                         50|                378|
|Colponemida            |Alveolata      |                          8|                378|
|Dinoflagellata         |Alveolata      |                       1355|                378|
|Ellobiopsidae          |Alveolata      |                          9|                363|
|InSedAlveolata         |Alveolata      |                         81|                375|
|MALV-I                 |Alveolata      |                        599|                378|
|MALV-II                |Alveolata      |                       2298|                378|
|MALV-III               |Alveolata      |                         80|                380|
|MALV-IV                |Alveolata      |                         47|                381|
|MALV-V                 |Alveolata      |                         13|                376|
|Perkinsidae            |Alveolata      |                        203|                379|
|Archamoebea            |Amoebozoa      |                          9|                385|
|Cavosteliida           |Amoebozoa      |                          8|                386|
|Dictyostelia           |Amoebozoa      |                          8|                417|
|Discosea               |Amoebozoa      |                        151|                492|
|Fractovitellida        |Amoebozoa      |                          3|                382|
|Gracilipodida          |Amoebozoa      |                         17|                389|
|InSedAmoebozoa         |Amoebozoa      |                         36|                351|
|Myxogastria            |Amoebozoa      |                         84|                436|
|Protosporangiida       |Amoebozoa      |                          5|                421|
|Protosteliida          |Amoebozoa      |                         20|                378|
|Schizoplasmodiidae     |Amoebozoa      |                         13|                392|
|Tubulinea              |Amoebozoa      |                         88|                388|
|Variosea               |Amoebozoa      |                          2|                418|
|Chlorodendrophyceae    |Archaeplastida |                          8|                380|
|Chlorophyceae          |Archaeplastida |                        156|                378|
|Chloropicophyceae      |Archaeplastida |                         17|                377|
|Glaucophyta            |Archaeplastida |                          5|                383|
|InSedArchaeplastida    |Archaeplastida |                        116|                379|
|Mamiellophyceae        |Archaeplastida |                        100|                377|
|Nephroselmis           |Archaeplastida |                         17|                381|
|Palmophyllophyceae     |Archaeplastida |                         19|                378|
|Pedinophyceae          |Archaeplastida |                          7|                374|
|Picocystophyceae       |Archaeplastida |                          1|                381|
|Picozoa                |Archaeplastida |                         30|                378|
|Prasino-Clade-IX       |Archaeplastida |                          8|                372|
|Pycnococcaceae         |Archaeplastida |                          3|                381|
|Pyramimonadales        |Archaeplastida |                         45|                379|
|Rhodophyceae           |Archaeplastida |                        387|                378|
|Streptophyta           |Archaeplastida |                        730|                380|
|Trebouxiophyceae       |Archaeplastida |                         81|                380|
|Ulvophyceae            |Archaeplastida |                         79|                378|
|Mantamonas             |CRuMS          |                          2|                385|
|Rigifilida             |CRuMS          |                          6|                388|
|Cryptomonadales        |Cryptista      |                        100|                376|
|Cyathomonadacea        |Cryptista      |                          4|                420|
|Kathablepharidacea     |Cryptista      |                         21|                377|
|Palpitomonas           |Cryptista      |                          1|                375|
|Ancyromonadida         |DeepBranching  |                         40|                380|
|Apusomonadida          |DeepBranching  |                        132|                382|
|Breviatea              |DeepBranching  |                         25|                380|
|Malawimonadidae        |DeepBranching  |                          1|                386|
|Diplonemea             |Discoba        |                         55|                538|
|Euglenida              |Discoba        |                        193|                633|
|Heterolobosea          |Discoba        |                         24|                486|
|InSedDiscoba           |Discoba        |                          1|                368|
|Jakobida               |Discoba        |                         17|                406|
|Kinetoplastea          |Discoba        |                        219|                534|
|Centroplasthelida      |Haptista       |                        160|                393|
|Pavlovales             |Haptista       |                         25|                380|
|Prymnesiophyceae       |Haptista       |                         63|                380|
|Fornicata              |Metamonada     |                         14|                360|
|Parabasalia            |Metamonada     |                        159|                267|
|Preaxostyla            |Metamonada     |                         11|                390|
|Aphelidiomycota        |Opisthokonta   |                         34|                379|
|Ascomycota             |Opisthokonta   |                        598|                379|
|BasalFungi             |Opisthokonta   |                         20|                382|
|Basidiobolomycota      |Opisthokonta   |                          2|                386|
|Basidiomycota          |Opisthokonta   |                        410|                380|
|Blastocladiomycota     |Opisthokonta   |                          8|                404|
|Calcarisporiellomycota |Opisthokonta   |                          3|                378|
|Choanoflagellata       |Opisthokonta   |                        239|                378|
|Chytridiomycota        |Opisthokonta   |                        183|                381|
|Entomophthoromycota    |Opisthokonta   |                         26|                424|
|Entorrhyzomycota       |Opisthokonta   |                          2|                382|
|Filasterea             |Opisthokonta   |                          2|                382|
|Glomeromycota          |Opisthokonta   |                         94|                381|
|Ichthyosporea          |Opisthokonta   |                         47|                378|
|InSedOpisthokonta      |Opisthokonta   |                         24|                380|
|Kickxellomycota        |Opisthokonta   |                          1|                339|
|MarineOpisthokonts     |Opisthokonta   |                         26|                377|
|Metazoa                |Opisthokonta   |                       7209|                394|
|Monoblepharomycota     |Opisthokonta   |                          7|                380|
|Mortierellomycota      |Opisthokonta   |                          5|                385|
|Mucoromycota           |Opisthokonta   |                         75|                388|
|NCLC1                  |Opisthokonta   |                         10|                380|
|Neocallimastigomycota  |Opisthokonta   |                          3|                381|
|Olpidiomycota          |Opisthokonta   |                          4|                382|
|Rotosphaerida          |Opisthokonta   |                         67|                380|
|Rozellomycota          |Opisthokonta   |                        120|                368|
|Zoopagomycota          |Opisthokonta   |                         66|                416|
|InSedEukaryota         |OtherEukaryota |                        386|                372|
|Nucleomorph            |OtherEukaryota |                         29|                387|
|Acantharea             |Rhizaria       |                        432|                368|
|Cercozoa               |Rhizaria       |                       1439|                390|
|Chlorarachnea          |Rhizaria       |                         54|                385|
|Foraminifera           |Rhizaria       |                         15|                713|
|InSedRhizaria          |Rhizaria       |                         34|                389|
|Polycystinea           |Rhizaria       |                        318|                382|
|RAD-A                  |Rhizaria       |                         64|                386|
|RAD-B                  |Rhizaria       |                         66|                384|
|RAD-C                  |Rhizaria       |                         28|                378|
|Aurearenophyceae       |Stramenopiles  |                          1|                396|
|Bicosoecida            |Stramenopiles  |                        169|                374|
|Bolidophyceae          |Stramenopiles  |                         34|                382|
|Cantina                |Stramenopiles  |                          1|                377|
|Chrysomerophyceae      |Stramenopiles  |                          4|                388|
|Chrysophyceae          |Stramenopiles  |                        262|                383|
|Developea              |Stramenopiles  |                          6|                386|
|Diatomea               |Stramenopiles  |                        822|                381|
|Dictyochophyceae       |Stramenopiles  |                         93|                389|
|Eustigmatales          |Stramenopiles  |                         20|                387|
|Hyphochytriales        |Stramenopiles  |                          5|                389|
|InSedStramenopiles     |Stramenopiles  |                        134|                386|
|Labyrinthulomycetes    |Stramenopiles  |                        411|                384|
|MAST-1                 |Stramenopiles  |                         28|                382|
|MAST-10                |Stramenopiles  |                          2|                380|
|MAST-11                |Stramenopiles  |                          3|                380|
|MAST-12                |Stramenopiles  |                         65|                386|
|MAST-16                |Stramenopiles  |                          1|                389|
|MAST-2                 |Stramenopiles  |                          4|                381|
|MAST-20                |Stramenopiles  |                          2|                380|
|MAST-22                |Stramenopiles  |                          8|                386|
|MAST-23                |Stramenopiles  |                          2|                388|
|MAST-24                |Stramenopiles  |                          2|                386|
|MAST-25                |Stramenopiles  |                          5|                376|
|MAST-3                 |Stramenopiles  |                        170|                383|
|MAST-4                 |Stramenopiles  |                          5|                380|
|MAST-6                 |Stramenopiles  |                         17|                386|
|MAST-7                 |Stramenopiles  |                         19|                377|
|MAST-8                 |Stramenopiles  |                         26|                386|
|MAST-9                 |Stramenopiles  |                         36|                379|
|MOCH-1                 |Stramenopiles  |                         21|                385|
|MOCH-2                 |Stramenopiles  |                         33|                383|
|MOCH-3                 |Stramenopiles  |                          2|                388|
|MOCH-4                 |Stramenopiles  |                          3|                388|
|MOCH-5                 |Stramenopiles  |                          7|                383|
|Opalinata              |Stramenopiles  |                         49|                379|
|Pelagophyceae          |Stramenopiles  |                         33|                385|
|Peronosporomycetes     |Stramenopiles  |                        103|                392|
|Phaeophyceae           |Stramenopiles  |                         24|                394|
|Phaeothamniophyceae    |Stramenopiles  |                          3|                388|
|Picophagus             |Stramenopiles  |                          3|                387|
|Pinguiophyceae         |Stramenopiles  |                          8|                389|
|Pirsoniales            |Stramenopiles  |                         21|                388|
|Placidida              |Stramenopiles  |                          6|                390|
|Raphidophyceae         |Stramenopiles  |                         10|                391|
|Schizocladia           |Stramenopiles  |                          1|                390|
|Synchromophyceae       |Stramenopiles  |                          4|                390|
|Synurophyceae          |Stramenopiles  |                         30|                383|
|Xanthophyceae          |Stramenopiles  |                         26|                392|
|Telonemia              |Telonemia      |                         31|                375|

## Versions

### v8

Several sequences discarded, complete reclassification of Fungi and other sequences.

Detailed changes:

  - Removed 77 sequences with clear errors. Discarded sequences can be found [here](db/old_versions/remove_v7_to_v8.txt).
  - Changed taxonomy in 912 sequences, especially within BasalFungi. Table with name changes can be found [here](db/old_versions/namechanges_v7_to_v8.txt).
  - One Fungi sequence added, [AY635841](db/old_versions/addseqs_v7_to_v8.txt).
  - Added information in the tax file with closest match to [pr2 database](https://pr2-database.org/).
  - Removed 'SLV' prefix from all SILVA sequences to use the original accession number.
  - Excavata no longer used, now separated into Discoba and Metamonada.
  - Added Telonemia supergroup.
  - Added DeepBranching supergroup (Ancyromonadida, Apusomonadida, Breviatea, and Malawimonadidae).

### v7

Changes in tax assignation and nomenclature. Additionaly, all U's in sequences changed to T's for consistency.

#### Changes in Chrysophyceae

|OTU         |New tax            |
|:-----------|:------------------|
|BMK7763     |InSedStramenopiles |
|BMK5345     |InSedStramenopiles |
|BMK5769     |InSedStramenopiles |
|SLVKF443034 |Synchromophyceae   |
|SLVAJ130893 |Synchromophyceae   |
|SLVKF925343 |Synchromophyceae   |
|SLVJN004145 |Synchromophyceae   |
|SLVU73225   |Synurophyceae      |
|BMK10049    |Synurophyceae      |
|SLVJN991181 |Synurophyceae      |
|SLVU73226   |Synurophyceae      |
|SLVJX946340 |Synurophyceae      |
|SLVU73219   |Synurophyceae      |
|SLVU73231   |Synurophyceae      |
|SLVGU935621 |Synurophyceae      |
|SLVU73222   |Synurophyceae      |
|SLVHF549063 |Synurophyceae      |
|SLVGU935623 |Synurophyceae      |
|SLVGU935633 |Synurophyceae      |
|SLVEF165118 |Synurophyceae      |
|SLVGU935624 |Synurophyceae      |
|SLVGU935628 |Synurophyceae      |
|SLVU73221   |Synurophyceae      |
|SLVGU935622 |Synurophyceae      |
|SLVJX946336 |Synurophyceae      |
|SLVGU325513 |Synurophyceae      |
|SLVHF549067 |Synurophyceae      |
|SLVHF549064 |Synurophyceae      |
|SLVGU325515 |Synurophyceae      |
|SLVGU067831 |Synurophyceae      |
|SLVAB749074 |Synurophyceae      |
|SLVJX455151 |Synurophyceae      |
|SLVAB622324 |Synurophyceae      |
|SLVHF549070 |Synurophyceae      |
|SLVKM590553 |Synurophyceae      |
|SLVAY919713 |Synurophyceae      |
|SLVAY919803 |Synurophyceae      |

#### Changes in Cryptomonadales

|OTU             |New tax     |
|:---------------|:-----------|
|SLVGAIN01011745 |Nucleomorph |
|SLVAJ420694     |Nucleomorph |
|SLVAJ420692     |Nucleomorph |
|SLVHF952607     |Nucleomorph |
|SLVAM901023     |Nucleomorph |

#### Change Other-Chlorophyta to InSedArchaeplastida

|OTU         |New tax            |
|:-----------|:------------------|
|MPN3330     |InSedArchaeplastida|

#### Changes in taxonomic groups nomenclature

|Old          |New       |
|:------------|:---------|
|Diatomeae    |Diatomea  |
|Blastocystis |Opalinata |

### v6

Changes in tax assignation for some misclassified references:

|OTU         |New tax                         |Old tax                            |
|:-----------|:-------------------------------|:----------------------------------|
|SLVKF651077 |Colponemida_Alveolata           |InSedAlveolata_Alveolata           |
|SLVKF211436 |Metazoa_Opisthokonta            |Protosporangiida_Amoebozoa         |
|SLVDQ267705 |Picocystophyceae_Archaeplastida |InSedArchaeplastida_Archaeplastida |
|SLVAM901018 |Nucleomorph_OtherEukaryota      |Cryptomonadales_Cryptista          |
|SLVJF791073 |Nucleomorph_OtherEukaryota      |Cryptomonadales_Cryptista          |
|SLVAY743950 |Metazoa_Opisthokonta            |Jakobida_Excavata                  |
|SLVAB597203 |BasalFungi_Opisthokonta         |Ascomycota_Opisthokonta            |
|SLVAB597204 |BasalFungi_Opisthokonta         |Ascomycota_Opisthokonta            |
|SLVFJ816018 |Rotosphaerida_Opisthokonta      |BasalFungi_Opisthokonta            |
|SLVL37733   |Ascomycota_Opisthokonta         |Basidiomycota_Opisthokonta         |
|SLVJN546121 |Ascomycota_Opisthokonta         |Basidiomycota_Opisthokonta         |
|BMK9285     |Ancyromonadida_OtherEukaryota   |Choanoflagellata_Opisthokonta      |
|SLVAB085614 |Schizocladia_Stramenopiles      |Phaeophyceae_Stramenopiles         |

### v5

Taxonomy adjusted to [Adl et al (2019)](https://doi.org/10.1111/jeu.12691). Name changes in the following groups:

|Old name             |Updated name       |
|:--------------------|:------------------|
|Choanomonada         |Choanoflagellata   |
|Colponema            |Colponemida        |
|X-Cell               |Perkinsidae        |
|Archamoebae          |Archamoebea        |
|Fractovitelliida     |Fractovitellida    |
|Schizoplasmodiida    |Schizoplasmodiidae |
|Charophyta           |Streptophyta       |
|Glaucocystophyceae   |Glaucophyta        |
|Nephroselmidophyceae |Nephroselmis       |
|Rhodophyta           |Rhodophyceae       |
|Goniomonas           |Cyathomonadacea    |
|Katablepharidae      |Kathablepharidacea |
|Kinetoplastida       |Kinetoplastea      |
|Centrohelida         |Centroplasthelida  |
|Pavlovophyceae       |Pavlovales         |
|Discicristoidea      |Rotosphaerida      |
|Acantharia           |Acantharea         |
|Chlorarachniophyta   |Chlorarachnea      |
|Bolidomonas          |Bolidophyceae      |
|Developayella        |Developea          |
|Diatomea             |Diatomeae          |
|Olisthodiscus        |Raphidophyceae     |
|Picophagea           |Picophagus         |
|Pinguiochrysidales   |Pinguiophyceae     |
|Pirsonia             |Pirsoniales        |

Also, Picozoa supergroup was changed to Archaeplastida, according to [Schön et al (2021)](https://doi.org/10.1101/2021.04.14.439778).

### v4

Sequence `MPN5387` (Pyramimonadales) was misclassified as MALV-II. Corrected in this version.

### v3

Updated Supergroups taxonomy:
  - 'Eukaryota' is now 'OtherEukaryota' to avoid misunderstandings.
  - 'Opisthokonta' is used instead of 'Obazoa'. Breviatea and Apusomonadida are then transferred to 'OtherEukaryota'.
  - Mantamonas and Rigifilida supergroup is changed from 'OtherEukaryota' to 'CRuMS'.

### v2

6 sequences with errors removed:

|Removed sequence                        |Error                               |
|:---------------------------------------|:-----------------------------------|
|`MPN7116_MAST-4_Stramenopiles`            |Missed 8 bases at position 60       |
|`BMK21470_Dinoflagellata_Alveolata`       |Had 4 gaps that should not be there |
|`MPN4866_Dinoflagellata_Alveolata`        |Missed 5-19 bases at position 220   |
|`BMK14604_Dictyochophyceae_Stramenopiles` |Seemed to be a chimera               |
|`MPN6667_Telonemia_Eukaryota`             |Missed 6 bp at position 280         | 
|`BMK17658_Cercozoa_Rhizaria`              |It had 6 gaps here and there        |

### v1

First version, used in *Mol Ecol Resour* [paper](https://doi.org/10.1111/1755-0998.13147).

## How was the database built?

The database was first built using 97% clustered V4 sequences from previous environmental high-throughput sequencing (HTS) studies in European coastal systems: 
Blanes Bay Microbial Observatory ([Giner et al., 2019](https://onlinelibrary.wiley.com/doi/full/10.1111/mec.14929)) and BioMarKs project ([Massana et al., 2015](https://sfamjournals.onlinelibrary.wiley.com/doi/full/10.1111/1462-2920.12955)), 
and the water column of the global ocean sampled during the 
Malaspina cruise ([Giner et al., 2020](https://www.nature.com/articles/s41396-019-0506-9)). 

Then, the database was complemented with trimmed 97% clustered V4 sequences from SILVA SSU 128 ([Quast et al., 2013](https://academic.oup.com/nar/article/41/D1/D590/1069277)) that 
were not found in environmental HTS datasets. This trimming was performed using cutadapt v1.16 ([Martin, 2011](https://journal.embnet.org/index.php/embnetjournal/article/view/200/479)) with the universal eukaryotic forward primer from [Stoeck et al. (2010)](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1365-294X.2009.04480.x) 
and reverse primer from [Balzano et al. (2015)](http://www.int-res.com/abstracts/ame/v74/n3/p263-277/), with an error rate of 0.2. 

All sequences were manually curated to discard possible chimeras and were classified 
at three taxonomic levels based on previous data, exhaustive inspection in multiple phylogenetic trees and iterative testing with environmental datasets to detect 
and correct problematic cases (i.e. distant references sequences retrieving the same mTag). These three levels were: 
  - OTU<sub>97</sub> level (Operational Taxonomic Units of sequences clustered at 97% similarity)
  - Taxonomic group (in general a formal Class)
  - Supergroup 

The largest effort was the classification at the taxonomic group level, 
which comprised 136 groups (see following section). The final *eukaryotesV4* database contains 25,849 sequences, 43% of which derive from environmental datasets.

