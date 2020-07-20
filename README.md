# BinBlaster

Provide either raw contigs or ORFs (in amino acid format) from a metagenome-assembled genome.
If raw contigs are provided, BinBlaster will use Prodigal to predict ORFs.

A reference protein dataset is also provided. Ideally, this should be the expansive nr database from NCBI, 
which can be downlaoded via: wget ftp://ftp.ncbi.nih.gov/blast/db/FASTA/nr.gz

This program will then BLAST each ORF against the reference database
(This takes about 30 minutes for a typical bacteria genome of ~4Mbp).

The program will then output a file in CSV format summarizing the dominant taxanomic groups matched to each contig.
This allows the user to visually inspect the data, seeing what the closest taxonomic group to each contig is.

Please see the Wiki for a brief tutorial!