Usage: iORI-Euk.exe [species/cell type] [query fasta file]

<1> iORI-Euk.exe is under the 'dist' folder.
<2> the parameter [species/cell type] is the following logogram for each species/cell type:
    H. sapiens(Hela cell) : H-Hela
    H. sapiens(MCF7 cell) : H-MCF7
    H. sapiens(K562 cell) : H-K562
    M. musculus(ES cell) : M-ES
    M. musculus(MEF cell) : M-MEF
    M. musculus(P19 cell) : M-P19
    D. melanogaster(Kc cell) : D-Kc
    D. melanogaster(S2 cell) : D-S2
    D. melanogaster(Bg3 cell) : D-Bg3
    A. thaliana: A
    P. pastoris: Pp
    S. pombe : Sp
    K. lactis: Kl
    S. cerevisiae : Scer
<3> the [query fasta file] format must be fasta sequence, Please refer to test1.fa, and each sequence length should be greater than 300bp and The [query fasta file] must be placed in the same directory as the iORI-Euk.exe..
<4> the result file is '*_final_result.txt', label '1' is 'ORI' and label '2' is 'non-ORI'.
<5> Running command to query H. sapiens(Hela cell): iORI-Euk.exe H-Hela test.fa
<5> Please use version 3.0 or above of Python.


