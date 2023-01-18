Hello, in this directory you will find all necessary non-read files used to run the analyses and generate the results described in the vAMPirus manuscript.


These files include:

	1. dinorna_meta_8_16_22.csv -> this is the metadata files used for the vAMPirus analysis
	2. dinoRNAV_vAMPirus_manuscript_dataset.config -> the configuration file used for the vAMPirus analysis


To run the same analysis using vAMPirus v2.1.0:

	1. Download SRA libraries associated with BioProject PRJNA923647
	2. Edit configuration file paths to metadata and databases (RVDB) used for taxonomy (can be downloaded using the vAMPirus startup script)
	3. Run vAMPirus with the following launch command:
	
		nextflow run vAMPirus.nf -c dinoRNAV_vAMPirus_manuscript_dataset.config -profile conda --Analyze --skipReport
		
		
		