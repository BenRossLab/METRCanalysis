Files in this repository to be run in the following order:
1. prelimNGS
2. prelimCulture
3. prelimCombo

REQUIRED INPUTS

prelimNGS requires the following as input:
1. A working repository (default ~/Desktop/Wannigan_METRC/ )
2. Folder within working repository containing all .fastq files (default ~/Desktop/Wannigan_METRC/raw/16S/ )
3. .csv file containing sample metadata listed with unique sampleIDs in first column (default ~/Desktop/Wannigan_METRC/raw/table_map.csv )
4. .csv file containing a list of sequences to be assigned to Homo sapiens (default ~/Desktop/Wannigan_METRC/raw/list_homoASVs.csv )

prelimCulture requires the following as input:

prelimCombo requires the following as input:

BRIEF DESCRIPTION OF PROCESS

prelimNGS processing includes:
1. standard DADA2 pipeline
2. assigning taxonomy using a modified silva_nr_v132 database
3. passing data into phyloseq object
4. correcting a few mis-identified important taxa
5. adding columns to mapping file based on calculations from processed sequencing data
6. final output = physeqR

prelimCulture processing includes:

prelimCombo processing includes:
