This repository contains alignment files and scripts to reproduce the paper,<b> "Congruence amidst discordance between sequence and protein-content based phylogenies of fungi"</b>

<b>1 TreePuzzle Analysis:</b><br> 
use the following script:   /home/ghx/puzzletree/puzzle   /home/ghx/puzzletree/spe27.phylip<br> 
notice:  you should change '/home/ghx/puzzletree/'  to  your own work space<br> 
Treepuzzle_outfile  is the output of the analysis.<br> 

<b>2 Matlab Clustering Analysis:</b><br> 
The file 'Data_for_clustering_analysis.mat'  contains the matrix data and label data for clustering analysis.<br> 
The sample Matlab Scripts are as follows(using cell wall proteins' matrix  for a sample analysis):<br> 
>> load Data_for_clustering_analysis.mat<br> 
>> Y = pdist(cellwall','correlation');<br> 
>> Z = linkage(Y,'average');<br> 
>> dendrogram(Z,'Labels',label)<br> 

After the analysis, you can save the tree file 'CellWallTree.pdf'.<br> 
Analysis of other matrixs is similar ,just change the input matrix data.<br> 




