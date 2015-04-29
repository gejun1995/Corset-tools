# Corset-tools
Companion scripts for annotation of Corset generated transcript clusters.

##fetchClusterSeqs.py
*Usage*: fetchClusterSeqs.py [-h] -i INFASTA -t TARGETCLUST [-o OUTFASTA] -c
                           CLUSTMAP

*Takes as input*: a list of target cluster names, transcript-to-cluster mapping
file generated by corset, and a fasta file containing transcript sequences.

*Returns*: Fasta file of transcripts belonging to query clusters, with Cluster
ID appended to their original sequence name.

*Required arguments*:
  -i INFASTA, --inFasta INFASTA
                        Multi fasta to extract subset from
  -t TARGETCLUST, --targetClust TARGETCLUST
                        Comma delimited file with target cluster names in
                        column one
  -c CLUSTMAP, --clustMap CLUSTMAP
                        Corset transcript-to-cluster mapping file.

*optional arguments*:
  -h, --help            show this help message and exit
  -o OUTFASTA, --outFasta OUTFASTA
                        Directory for new sequence file to be written to.