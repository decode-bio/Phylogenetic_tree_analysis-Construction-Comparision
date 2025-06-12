
# Objective
Construction and comparison of phylogenetic trees for the obtained homologs from BLAST analysis.

# 1. Selecting the Gene of Interest
For the analysis of the sequence, here I am taking the Homo sapiens cytochrome C oxidase as gene or nucleotide sequence. Cytochrome oxidase is a terminal member of the electron transport chain in mitochondria and many bacteria. It catalyzes the reduction of molecular oxygen in a concerted four-electron transfer step, and uses the free energy of this reaction to establish a proton gradient across the membrane(reference :Cytochrome C Oxidase - an overview | ScienceDirect Topics).

# 2. Pairwise Alignment Using BLASTn
Downloaded the gene sequence of interest from NCBI in fasta format.Copied only the sequence and putting it in BLASTn for the Alignment. For further analysis selected the five genes from different species for the tree construction. Along with our Query sequence.

# 3. MSA (Multiple sequence Alighment)
Fetched the five highly similar sequences from different species for Multiple sequence Alignment(MSA). MSA is performed using CLUSTAL Omega, MUSCLE and T-COFFEE.

# 4. Comparision of MSA tools used
![image](https://github.com/user-attachments/assets/a541dfe7-5187-43a7-bf17-0a2cf1a7ae02)

If we consider all the factors together the coverage and percentage identity so we can see from the above result that in our case, Clustal omega and Muscle provides the better results in comparison to the T-CoFFee. But as we have to take one for further phylogenetic tree analysis, I will go for the MUSCLE.

# 5. Selection for Phylogenetic Analysis
Decision: Use the MSA result from the tool that provided the best alignment quality based on criteria. MUSCLE is selected as it gives fast and accurate results and also shows minimal misalignments and optimal conservation of known motifs, judged both visually and by quantitative metrics.

# 6. Using MEGA 12 for phylogenetic tree construction using all five methods.
MEGA:Molecular Evolutionary Genetics Analysis (MEGA) is computer software for conducting statistical analysis of molecular evolution and for constructing phylogenetic trees. There are five different methods for the construction of the tree those are as follows: 
* a) Maximum Likelihood (ML)
* b) Neighbor-Joining (NJ)
* c) Minimum Evolution (ME)
* d) Maximum Parsimony (MP)
* e) UPGMA (Unweighted Pair Group Method with Arithmetic Mean)

# a) Maximum Likelihood (ML)
![image](https://github.com/user-attachments/assets/dcb472ff-4bc6-4cfb-acf0-91ccd28dc26c)

Here, based on the length we can state that the longer the horizontal length the larger is the genetic change. The Value 0.01 represents the amount of genetic change. The number across the nodes represents the measure of support for the node. Higher the number higher will be the support. Maximum can be 100. The node representing the 99 support because both species are from the same genus i.e. Pongo.

# b) Neighbor-Joining (NJ)
![image](https://github.com/user-attachments/assets/ceae115f-d4b9-4656-aff2-9439e96115d0)

From the above graph we can say that the amount of genetic change is 0.01.Here the maximum support is 97, shown across the genus of Pan and Gorilla species. 

# c) Minimum Evolution (ME)
![image](https://github.com/user-attachments/assets/de145a3c-6eda-4591-b692-405ae5a815f8)

From the above graph we can say that the amount of genetic change is 0.01.Here the maximum support is 96, shown across the genus of Pan and Gorilla species. 

# d) Maximum Parsimony (MP)
![image](https://github.com/user-attachments/assets/9cd3abf7-612e-4d0e-8b4d-6c495d7c2a49)

Here it is showing the change in genetic amount is 2.0 which is maximum in comparison of all other four methods. In this method it does not unrooted the Homo sapiens gene unlike other four.

#  e) UPGMA (Unweighted Pair Group Method with Arithmetic Mean)
![image](https://github.com/user-attachments/assets/867256f8-3d22-44a8-a597-60344a5e6eba)

Here also the amount of genetic change is 0.01. Here also it is showing the close relationship between the Gorilla and Pan species. Showing better support between the Pongo Pygmaeus and Pongo abelii in comparison to the Neighbor joining and Minimum evolution methods.

# Conclusion
Comparing all the five results obtained using different methods, the Maximum likelihood method gave the best results for the evolution. Because if we compare all the five, the Maximum parsimony shows the maximum amount of genetic change i.e. 2.0 percentage. Whereas as compared to the other three the maximum likelihood gives us evolutionary accurate and reliable results.It gives us the results in log value which is more reliable as compared to the others method. Hence most of the time we consider it as construction of a phylogenetic tree due to its statistical validity.

Thank you so much for you time.
Any valuable input is appreciated.
Contact me at @ sneha.biocode@gmail.com
