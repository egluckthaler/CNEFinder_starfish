MIM: Maximal Inexact Matches
===

<b>Description</b>: Given two genomes r and q, and a reference and query gene or coorindate valyes, MIM finds CNEs matches between either the positions of the provided genes or coordinate values of the respective chromosomes of r and q.

<b>Installation</b>: To compile MIM, please follow the instructions given in file INSTALL.
```
 Usage: MIM <options>
 Standard (Mandatory):
  -r, --ref-genome-file		<str>		FASTA reference genome filename.
  -q, --query-genome-file	<str>		FASTA query genome filename.
  -e, --exons-ref-file		<str>		GTF/GFF exon coordinates for reference genome filename.
  -f, --exons-query-file	<str>		GTF/GFF exon coordinates for query genome filename.
  -l, --min-seq-length		<int>		Minimum length of match.
  -k, --sim-threshold		<dbl>		Threshold of similarity between sequences.
  -o, --output-file		<str>		Output filename with CNEs identified.

  Either 1. or 2.
    1.Search using gene name:
    -g, --ref-gene-file		<str>		GTF/GFF filename containing gene data for reference genome.
    -n, --ref-gene-name		<str>		Name of gene in reference genome in which CNEs will be identified.
    -j, --query-gene-file	<str>		GTF/GFF filename containing gene data for query genome.
    -m, --query-gene-name	<str>		Name of gene in query genome in which CNEs will be identified.

    2.Search using coordinates:
    -y, --ref-chrom		<str>		Chromsome of reference genome.
    -z, --query-chrom		<str>		Chromosome of query genome.
    -a, --ref-start		<int>		Start CNE search from this position of reference sequence.
    -b, --ref-end		<int>		End CNE search at this position of reference sequence.
    -c, --query-start		<int>		Start CNE search from this position of query sequence.
    -d, --query-end		<int>		End CNE search at this position of query sequence.

 Optional:
  -p, --repet-regions		<int>		Choose 1 to filter repetitive regions of genomes or 0 otherwise. Default:1.	
  -v, --rev-complement		<int>		Choose 1 to compute CNEs for reverse complement or 0 otherwise. Default:0.
  -x, --remove-overlaps		<int>		Choose 1 to remove overlapping CNEs or 0 otherwise. Default:1.

 Number of threads:
  -T, --threads			<int>		Number of threads to use. Default:1. 
```

<b>License</b>: GNU GPLv3 License; Copyright (C) 2017 Lorraine A. K. Ayad, Solon P. Pissis, Dimitris Polychronopoulos

