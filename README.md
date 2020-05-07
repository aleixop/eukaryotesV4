# *eukaryotesV4* database

[![DOI](https://zenodo.org/badge/198411321.svg)](https://zenodo.org/badge/latestdoi/198411321)

*eukaryotesV4* is a curated database of V4 region of 18S rDNA. It was built to extract and taxonomically classify short metagenomic reads (mTags).  

You can download it in [fasta](db/eukaryotesV4_v2.fasta) format or [.txt file](db/eukaryotesV4_tax_v2.txt) with additional information.
A version with headers formatted to work with `dada2` is also available [here](db/eukaryotesV4_v2_dada2.fasta).

## Citation

Obiol, A., Giner, C.R., Sánchez, P., Duarte, C.M., Acinas, S.G. and Massana, R. [A metagenomic assessment of microbial eukaryotic diversity in the global ocean](https://doi.org/10.1111/1755-0998.13147). *Mol Ecol Resour*. 2020; 20: 718– 731. doi: 10.1111/1755-0998.13147

## Versions

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

## Overview of the database

Here is a summary table with the taxonomic groups contained in *eukaryotesV4* database v1.

|Group                |Supergroup     | OTU<sub>97</sub> sequences| Median length (bp)|
|:--------------------|:--------------|---------------:|------------------:|
|Apicomplexa          |Alveolata      |             615|                370|
|Ciliophora           |Alveolata      |            1975|                369|
|Colpodellida         |Alveolata      |              28|                378|
|Colponema            |Alveolata      |               7|                379|
|Dinoflagellata       |Alveolata      |            1384|                378|
|Ellobiopsidae        |Alveolata      |               9|                363|
|InSedAlveolata       |Alveolata      |             138|                377|
|MALV-I               |Alveolata      |             605|                378|
|MALV-II              |Alveolata      |            2306|                378|
|MALV-III             |Alveolata      |              82|                380|
|MALV-IV              |Alveolata      |              47|                381|
|MALV-V               |Alveolata      |              14|                376|
|Perkinsidae          |Alveolata      |              94|                379|
|X-Cell               |Alveolata      |              56|                403|
|Archamoebae          |Amoebozoa      |               9|                385|
|Cavosteliida         |Amoebozoa      |               8|                386|
|Dictyostelia         |Amoebozoa      |               8|                417|
|Discosea             |Amoebozoa      |             152|                492|
|Fractovitelliida     |Amoebozoa      |               3|                382|
|Gracilipodida        |Amoebozoa      |              17|                389|
|InSedAmoebozoa       |Amoebozoa      |              37|                351|
|Myxogastria          |Amoebozoa      |              84|                436|
|Protosporangiida     |Amoebozoa      |               6|                422|
|Protosteliida        |Amoebozoa      |              20|                378|
|Schizoplasmodiida    |Amoebozoa      |              13|                392|
|Tubulinea            |Amoebozoa      |              87|                388|
|Charophyta           |Archaeplastida |             730|                380|
|Chlorodendrophyceae  |Archaeplastida |               8|                380|
|Chlorophyceae        |Archaeplastida |             156|                378|
|Chloropicophyceae    |Archaeplastida |              18|                376|
|Glaucocystophyceae   |Archaeplastida |               2|                384|
|Glaucophyta          |Archaeplastida |               3|                382|
|InSedArchaeplastida  |Archaeplastida |             122|                379|
|Mamiellophyceae      |Archaeplastida |             100|                377|
|Nephroselmidophyceae |Archaeplastida |              17|                381|
|Other-Chlorophyta    |Archaeplastida |               1|                380|
|Palmophyllophyceae   |Archaeplastida |              19|                378|
|Pedinophyceae        |Archaeplastida |               7|                374|
|Prasino-Clade-IX     |Archaeplastida |               8|                372|
|Pycnococcaceae       |Archaeplastida |               3|                381|
|Pyramimonadales      |Archaeplastida |              44|                379|
|Rhodophyta           |Archaeplastida |             388|                378|
|Trebouxiophyceae     |Archaeplastida |              81|                380|
|Ulvophyceae          |Archaeplastida |              79|                378|
|Cryptomonadales      |Cryptista      |             109|                376|
|Goniomonas           |Cryptista      |               4|                420|
|Katablepharidae      |Cryptista      |              21|                377|
|Palpitomonas         |Cryptista      |               1|                375|
|Ancyromonadida       |Eukaryota      |              39|                380|
|InSedEukaryota       |Eukaryota      |             324|                358|
|Malawimonadidae      |Eukaryota      |               1|                386|
|Mantamonas           |Eukaryota      |               2|                385|
|Nucleomorph          |Eukaryota      |              18|                390|
|Picozoa              |Eukaryota      |              31|                378|
|Rigifilida           |Eukaryota      |               6|                388|
|Telonemia            |Eukaryota      |              32|                376|
|Diplonemea           |Excavata       |              56|                538|
|Euglenida            |Excavata       |             194|                633|
|Fornicata            |Excavata       |              14|                360|
|Heterolobosea        |Excavata       |              24|                486|
|Jakobida             |Excavata       |              18|                406|
|Kinetoplastida       |Excavata       |             220|                534|
|Parabasalia          |Excavata       |             159|                267|
|Preaxostyla          |Excavata       |              11|                390|
|Centrohelida         |Haptista       |             159|                393|
|Pavlovophyceae       |Haptista       |              25|                380|
|Prymnesiophyceae     |Haptista       |              63|                380|
|Apusomonadida        |Obazoa         |             132|                382|
|Ascomycota           |Obazoa         |             601|                379|
|BasalFungi           |Obazoa         |             704|                381|
|Basidiomycota        |Obazoa         |             416|                380|
|Breviatea            |Obazoa         |              24|                380|
|Choanomonada         |Obazoa         |             241|                378|
|Discicristoidea      |Obazoa         |              39|                380|
|Filasterea           |Obazoa         |               5|                381|
|Ichthyosporea        |Obazoa         |              47|                378|
|InSedObazoa          |Obazoa         |              67|                381|
|MarineOpisthokonts   |Obazoa         |              27|                377|
|Metazoa              |Obazoa         |            7220|                394|
|Acantharia           |Rhizaria       |             434|                367|
|Cercozoa             |Rhizaria       |            1440|                390|
|Chlorarachniophyta   |Rhizaria       |              56|                384|
|Foraminifera         |Rhizaria       |              15|                713|
|InSedRhizaria        |Rhizaria       |              35|                389|
|Polycystinea         |Rhizaria       |             318|                382|
|RAD-A                |Rhizaria       |              64|                386|
|RAD-B                |Rhizaria       |              66|                384|
|RAD-C                |Rhizaria       |              28|                378|
|Aurearenophyceae     |Stramenopiles  |               1|                396|
|Bicosoecida          |Stramenopiles  |             165|                374|
|Blastocystis         |Stramenopiles  |              45|                379|
|Bolidomonas          |Stramenopiles  |              34|                382|
|Cantina              |Stramenopiles  |               1|                378|
|Chrysomerophyceae    |Stramenopiles  |               4|                388|
|Chrysophyceae        |Stramenopiles  |             299|                383|
|Developayella        |Stramenopiles  |               6|                386|
|Diatomea             |Stramenopiles  |             822|                381|
|Dictyochophyceae     |Stramenopiles  |              94|                389|
|Eustigmatales        |Stramenopiles  |              20|                387|
|Hyphochytriales      |Stramenopiles  |               5|                389|
|InSedStramenopiles   |Stramenopiles  |             134|                386|
|Labyrinthulomycetes  |Stramenopiles  |             414|                384|
|MAST-1               |Stramenopiles  |              28|                382|
|MAST-10              |Stramenopiles  |               2|                380|
|MAST-11              |Stramenopiles  |               3|                380|
|MAST-12              |Stramenopiles  |              65|                386|
|MAST-16              |Stramenopiles  |               1|                389|
|MAST-2               |Stramenopiles  |               4|                381|
|MAST-20              |Stramenopiles  |               2|                380|
|MAST-22              |Stramenopiles  |               8|                386|
|MAST-23              |Stramenopiles  |               2|                388|
|MAST-24              |Stramenopiles  |               2|                386|
|MAST-25              |Stramenopiles  |               5|                376|
|MAST-3               |Stramenopiles  |             170|                383|
|MAST-4               |Stramenopiles  |               6|                380|
|MAST-6               |Stramenopiles  |              17|                386|
|MAST-7               |Stramenopiles  |              19|                377|
|MAST-8               |Stramenopiles  |              26|                386|
|MAST-9               |Stramenopiles  |              36|                379|
|MOCH-1               |Stramenopiles  |              21|                385|
|MOCH-2               |Stramenopiles  |              33|                383|
|MOCH-3               |Stramenopiles  |               2|                388|
|MOCH-4               |Stramenopiles  |               3|                388|
|MOCH-5               |Stramenopiles  |               7|                383|
|Olisthodiscus        |Stramenopiles  |               1|                387|
|Opalinata            |Stramenopiles  |               4|                396|
|Pelagophyceae        |Stramenopiles  |              34|                384|
|Peronosporomycetes   |Stramenopiles  |             104|                392|
|Phaeophyceae         |Stramenopiles  |              25|                394|
|Phaeothamniophyceae  |Stramenopiles  |               3|                388|
|Picophagea           |Stramenopiles  |               3|                387|
|Pinguiochrysidales   |Stramenopiles  |               8|                389|
|Pirsonia             |Stramenopiles  |              21|                388|
|Placidida            |Stramenopiles  |               6|                390|
|Raphidophyceae       |Stramenopiles  |               9|                391|
|Xanthophyceae        |Stramenopiles  |              25|                393|
