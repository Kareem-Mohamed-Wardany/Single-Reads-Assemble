# Single-Reads-Assemble
<p>you should assemble two types of reads using the De Bruijn graph representation and the Eulerian path to obtain the
original sequence from that representation.</p>
<b>Short reads with the same size</b>

Input : Your program should be able to read a file.
The first line would be: - the length of the sequences.
                         - Each read will take one.
Output : The program then outputs the assembled sequence to the screen.


<h1>Explain</h1>

<b>#READS</b> 
CTTA
ACCA
TACC
GGCT
GCTT
TTAC

<b>#GRAPH</b> 
CTT --> TTA
ACC --> CCA(E)
TAC --> ACC
(S)GGC --> GCT
GCT --> CTT
TTA --> TAC


<b>#PATHS</b> 
GGC -> GCT -> CCT -> TTA -> TAC -> ACC -> CCA
Get first 3 letters in first one and then get last letter in others

the final result should be like 
Genome = GGCTTACCA
