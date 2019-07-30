### Generic differential expression setup
#### Kate Lee 2019

Setup folders and scripts for a differential expression analysis. The pipeline includes QC with fastqc and trimmomatic, read counts with Salmon and a differential expression analysis with DESeq.

#### REQUIREMENTS:
- config.txt 
    - config file with 7 columns (as in DESeq), no headers in file. 
    - contains: species, centre,  assay, run_num(e.g. when samples sent for re-sequencing), lane, sample,  experiment,  run(illumina run fq base filename), condition(tissue).
- DESeq2_compare.txt with three columns for (species, condition, ref_condition). No headers in file.

#### USAGE
```{perl}
perl setup_DESeq_analysis.pl <config.txt> <DESeq2_compare.txt> <optional:raw_data_foldername>            
```
(note, the raw data folder default name is 0_raw_data)
Go to the 




