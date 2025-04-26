The goal of this fork is to get rid of the very annoying step of regularly building
the Id_to_taxid 48 gigabyte file.
This is useless if you run the blast in a particular -outfmt "7 ..." asking for taxid to be reported by Blastn

Obviously this will work only on NCBI's premade blast banks

/opt/bp/blastn -task blastn -query fs.fa -db /data/dbs/bdbs/BB/16S_ribosomal_RNA -outfmt "7 qacc sacc pident evalue bitscore staxid"

these are the only used elements required from a blastn output
