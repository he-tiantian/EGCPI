EGCPI: an evolutionary graph clustering algorithm for protein complex identification. The software in this repository is developed based on the following article: 
T. He, and K.C.C. Chan, "Evolutionary Graph Clustering for Protein Complex Identification," IEEE/ACM Transactions on Computational Biology and Bioinformatics, vol. 15, no. 3, pp. 892-904, 2018.

How to use EGCPI to detect protein complexes in the PPI network
Before running the executable file (EGCPI_v1.0.jar), please prepare the processed PPI network data, and file of configurations, and put them into the same directory where the executable file is.

The processed PPI network data contain the following files:
1)matrix of degree of topological similarity (default: SSG.csv)
2)matrix of degree of attribute homogeneity (default: ASG.csv)
3)adjaceny matrix of the PPI network (default: graph.csv)
4)network information (default: statistics)
5)protein information (default: vertex)
In order to help users to transform the PPI network data into the compatible format that is used by EGCPI. A example of processed PPI network data obtained from the Collins data set has been offered together with the executable file. Please check them for detail. To collect all the datasets used in the above paper, please go to .\PPI-Datasets to download them.

The file of configurations (EGCPI.config) is used to set the parameters before EGCPI runs. A default setting which may ensure EGCPI perform robustly is offered together with the executable file. The format of the file can be checked in GCPI.config. And the users may configure them accordingly. For most of the case, the users can adjust Lambda (ranges from 0 to 1) and ovMax (ranges from 0 to 1) to obtain different results. As other settings, they bring a limited impact on the results of identified protein complexes.

Identifying Protein complexes

After doulble clicking the .jar file, a simple graphical interface will be shown to the user. All that one needs to do is to click the "start detection" button and wait for the results (this won't take a long time). After the detection is finished, EGCPI will save all the deteced protein complexes int a file which is named as Cluster.txt in default and save all the information on the the execution incuding fitness value, running time, etc into a log file named as log.txt in default. The user may make use them for their own experiments accordingly.

Notice: This software is permitted to use only for research and non-commercial activities. If you have any question, please feel free to contact us via tiantian.he@outlook.com.

At last, thanks very much for using EGCPI.
