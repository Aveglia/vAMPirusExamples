Hello, in this directory you will find all necessary non-read files used to run the analyses and generate the results described in the vAMPirus manuscript.


These files include:

	1. portalprotein_meta.csv -> this is the metadata files used for the vAMPirus analysis
	2. FrantzenHolo_2019_vampirus.config -> the configuration file used for the vAMPirus analysis


To run the same analysis using vAMPirus v2.1.0:

	1. Data can be requested from authors
	2. Edit configuration file paths to metadata and databases (virus refseq) used for taxonomy (can be downloaded using the vAMPirus startup script)
	3. Run vAMPirus with the following launch command (skip command used to reduce run time):
	
		nextflow run vAMPirus.nf -c dinoRNAV_vAMPirus_manuscript_dataset.config -profile conda --Analyze --ncASV --aminoTClust --resume --skipReport
		
