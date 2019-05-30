# OrfTxdb
Orf virus sequence forged in BSgenome format


#installaltion

Download the tar file and you can install it manually.


#USE

library (OrfTxdb)
> dna <- OrfTxdb
>dna

 Orf virus genome:
 
 organism: Orfv (Orf virus)
 
 provider: NCBI
 
 provider version: 1.0.0
 
release date: Jan.2004

 release name: Orf virus strain OV-IA82
 
 1 sequences:
 
   orfv       
   
(use 'seqnames()' to see all the sequence names, use the '$' or '[[' operator to
access a given sequence)

> seqlengths(dna)

  orfv 
  
137241 
> seqnames(dna)

[1] "orfv"

> dna$orfv

  137241-letter "DNAString" instance
  
seq: CGAGAACGCGGACCAGGAGTTCCTGCGGGAGGAGCTACG...CGTAGCTCCTCCCGCAGGAACTCCTGGTCCGCGTTCTCG

> letterFrequency (dna$orfv, "CG", as.prob = TRUE)

      C|G 
      
0.6433719 