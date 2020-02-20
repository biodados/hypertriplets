# HyperTriplets - Triplet-based supertree generator


## Introduction:

	HyperTriplets is a phylogenetic tool that makes a supetree based on triplets 
	analysis. It takes as input several gene trees in Newick format. 


## Prerequisites:

	Unix Platform;
	PERL;


## For impatients:

	> tar -zxvf HyperTriplets_vXXX.tgz
	> cd hypertriplets
	> ./hypertriplets_db -treedir <tree_directory>
	> ./hypertriplets_analayse -table <hash_file> 

## For detailed description of HyperTriplets parameters:

	> ./hypertriplets_db -man
	> ./hypertriplets_analyse -man

	
## Installation:

	HyperTriplets is ready to use  in  most  of  Unix  Platform.  But  it  only 
	works if the  folder  lib/  that follow this script is  in  the  same 
	location. If you want to freely run HyperTriplets  in  other  location, add  
	the HyperTriplets folder  into  the  environment  variable  by  using,  for 
	example, the following commands:
	
	> echo "export PATH=$PATH:/path/to/program/hypertriplets/" >> ~/.bashrc
	> source ~/.bashrc

	
## Running with sample files:

	In the hypertriplets directory try the following commands
	> ./hypertriplets_db -treedir sample_trees/ -out sample_db.tab
	> ./hypertriplets_analayse -table sample_db.tab -out sample_result


## Outputs:

	hypertriplets_db: a hash file containing the taxonomic and distance information.
	
	hypertriplets_analyse:
      *.nwk:        a supertree in Newick format.
      *_itol.txt:   a file containing a pie chart dataset with branch support values.
                    Upload the supertree and this file to iToL.

