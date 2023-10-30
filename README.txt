# iORI-Euk
## Abstract
The locations of the initiation of genomic DNA replication are defined as origins of replication sites (ORIs), which regulate the onset of DNA replication and play significant roles in the DNA replication process. The study of ORIs is essential for understanding the cell-division cycle and gene expression regulation. Accurate identification of ORIs will provide important clues for DNA replication research and drug development by developing computational methods. In this paper, the first integrated predictor named iORI-Euk was built to identify ORIs in multiple eukaryotes and multiple cell types. In the predictor, seven eukaryotic (Homo sapiens, Mus musculus, Drosophila melanogaster, Arabidopsis thaliana, Pichia pastoris, Schizosaccharomyces pombe and Kluyveromyces lactis) ORI data was collected from public database to construct benchmark datasets. Subsequently, three feature extraction strategies which are k-mer, binary encoding and combination of k-mer and binary were used to formulate DNA sequence samples. We also compared the different classification algorithms’ performance. As a result, the best results were obtained by using support vector machine in 5-fold cross-validation test and independent dataset test. Based on the optimal model, an online web server called iORI-Euk (http://lin-group.cn/server/iORI-Euk/) was established for the novel ORI identification.

## Usage
iORI-Euk.exe [species/cell type] [query fasta file]

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

## citation
Fu-Ying Dao, Hao Lv, Hasan Zulfiqar, Hui Yang, Wei Su, Hui Gao, Hui Ding, Hao Lin*. (2021) A computational platform to identify origins of replication sites in eukaryotes. Briefings in Bioinformatics, 22(2): 1940–1950. 

## contact
fuying.dao@ntu.edu.sg

