# Introduction

This repository contains trained reference sets that can be used with the Ribosomal Database Project classifier (Wang et al., 2007) to taxonomically assign diatom rbcL cpDNA sequences.  The latest releases can be downloaded from https://github.com/terrimporter/rbcLdiatomClassifier/releases

## Note

This classifier is suitable for classifying diatom rbcL sequences to genus rank.  To classify a broader diversity of taxa, there is a Eukaryote rbcL reference set available at https://github.com/terrimporter/rbcLClassifier .

## How to cite

If you use this rbcL diatom reference set in a publication, please link to this page in your methods section and cite the diatom barcode database:

Rimet, F., Chaumeil, P., Keck, F., Kermarrec, L., Vasselon, V., Kahlert, M., Franc, A., Bouchez, A. 2016.  R-Syst::diatom: an open-access and curated barcode database for diatoms and fr3eshwater monitoring.  Database: baw016. 

If you use this reference set with the RDP classifier please also cite:

Wang et al. (2007) Naïve Bayesian classifier for rapid assignment of rRNA sequences into the new bacterial taxonomy. Applied and Environmental Microbiology, 73: 5261.

# Releases

### SSU diatom v1.0

Created from the INRA R-Syst::diatom v7.1 dataset available at https://data.inra.fr/dataset.xhtml?persistentId=doi%3A10.15454%2FTOMBYZ (Rimet et al., 2016).  This version contains 3504 reference sequences and 1432 taxa at all ranks.

**Taxonomic assignment results should be filtered according to their bootstrap support values to reduce false positive assignments.**  Cutoffs are based on leave-one-sequence-out testing of non-singleton genera. Here we recommend MINIMUM bootstrap cutoffs according to query length and assignment rank.  Assuming your query sequences are represented in the reference set, using the cutoffs presented in the first table below should ensure 99% accuracy.  If you wish to cast a wider net, you can use the second table below for 95% accuracy.

#### Bootstrap support cutoffs, 99% accuracy:

Rank | Full | 400 bp | 300 bp | 200 bp | 100 bp
--- |:---:|:---:|:---:|:---:|:---:
Domain | 0 | 0 | 0 | 0 | 0
Kingdom | 0 | 0 | 0 | 0 | 0
Subkingdom | 0 | 0 | 0 | 0 | 0
Phylum | 0 | 0 | 0 | 0 | 0
Class | 0 | 40 | 40 | 50 | 70
Order | 50 | 60 | 50 | 60 | 90
Family | 70 | 60 | 60 | 60 | NA
Genus | NA | 95 | 80 | 90 | NA
Species | NA | NA | NA | NA | NA

NA = No cutoff available will result in 99% correct assignments

#### Bootstrap support cutoffs, 95% accuracy:

Rank | Full | 400 bp | 300 bp | 200 bp | 100 bp
--- |:---:|:---:|:---:|:---:|:---:
Domain | 0 | 0 | 0 | 0 | 0
Kingdom | 0 | 0 | 0 | 0 | 0
Subkingdom | 0 | 0 | 0 | 0 | 0
Phylum | 0 | 0 | 0 | 0 | 0
Class | 0 | 0 | 0 | 0 | 10
Order | 0 | 0 | 0 | 0 | 50
Family | 0 | 0 | 0 | 20 | 50
Genus | 0 | 30 | 20 | 40 | 60
Species | NA | NA | NA | NA | NA

NA = No cutoff available will result in 95% correct assignments

# References

Rimet, F., Chaumeil, P., Keck, F., Kermarrec, L., Vasselon, V., Kahlert, M., Franc, A., Bouchez, A. 2016.  R-Syst::diatom: an open-access and curated barcode database for diatoms and fr3eshwater monitoring.  Database: baw016. 

Wang, Q., Garrity, G. M., Tiedje, J. M., & Cole, J. R. (2007). Naive Bayesian Classifier for Rapid Assignment of rRNA Sequences into the New Bacterial Taxonomy. Applied and Environmental Microbiology, 73(16), 5261–5267. Available from https://sourceforge.net/projects/rdp-classifier/

# Acknowledgements

We acknowledge support from the Canadian federal Genomics Research & Development Initiative (GRDI), Metagenomics-Based Ecosystem Biomonitoring (Ecobiomics) project.

Last updated: February 11, 2020
