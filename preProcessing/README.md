Files in this repository to be run in the following order:
1. prelimNGS
2. prelimCulture
3. prelimCombo

REQUIRED INPUTS

prelimNGS requires the following as input:
1. A working repository (default "~/Desktop/Wannigan_METRC/")
2. "~/Desktop/Wannigan_METRC/raw/16S/" : a folder within working repository containing all .fastq files
3. "~/Desktop/Wannigan_METRC/raw/table_map.csv" : a data table containing sample metadata listed with unique sampleIDs in first column
4. "~/Masters/silva_nr_v132_train_set_RossMod.fa" : a reference taxonomy database
5. "~/Desktop/Wannigan_METRC/raw/list_homoASVs.csv" : a list of sequences to be assigned to Homo sapiens

prelimCulture requires the following as input:

prelimCombo requires the following as input:
1. "~/Desktop/Wannigan_METRC/raw/table_map.csv" : a data table containing metadata for all samples
2. "~/Desktop/Wannigan_METRC/outputPrelim/table_compileCulture.csv" : a data table containing compiled culture data
3. "~/Desktop/Wannigan_METRC/raw/table_spp.csv" : a data table containing species descriptions
4. 
5. "~/Desktop/Wannigan_METRC/outputPrelim/physeqR.RData : a phyloseq object containing paired and trimmed 16S reads
6. "~/Desktop/Wannigan_METRC/outputPrelim/table_cultureBase.csv" : a data table containing baseline culture data
7. "~/Desktop/Wannigan_METRC/outputPrelim/table_cultureFU.csv" : a data table containing follow-up culture data
8. 
9. "~/Masters/color_palettes.R" : an .R file containing user-defined color palettes

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

All code in the METRCanalysis repository was written by Emily Ann McClure. No AI was used at any stage in writing this code.

