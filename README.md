# MRM-Ion Pair Finder

## Introduction
Pseudotargeted metabolomics is a novel method that perform high coverage metabolomics analysis based on UHPLC-TQMS. MRM-Ion Pair Finder software is an independently developed and written program in our laboratory for large-scale selection of MRM transitions for pseudotargeted metabolomics. The Matlab (Version 7.14.739, R2012a,64-bit) is used. MRM-Ion Pair Finder v2.0 is improved on the basis of the original version, which simplifies the program and improves the running efficiency. Matlab language (R2018b, 64-bit) is used. To make MRM-Ion Pair Finder can be used by more researchers, we also provide a version based on R.

## Development
MRM-Ion Pair Finder is used to automatically and systematically define MRM transitions from untargeted metabolomics data. Our research group first introduced the concept of pseudotargeted metabolomics using the retention time locking GC-MS-selected ions monitoring in 2012. The pseudotargeted metabolomics method was extended to LC-MS in 2013. To define ion pairs automatically and systematically, the in-house software “Mul-tiple Reaction Monitoring-Ion Pair Finder (MRM-Ion Pair Finder)” was developed, which made defining of the MRM transitions for untargeted metabolic profiling easier and less time consuming. Recently, MRM-Ion Pair Finder was updated to version 2.0. The new version is more convenient, consumes less time and is also suitable for negative ion mode. And the function of MRM-Ion Pair Finder is also performed in R so that users have more options when using the development of pseudotargeted method.

## How to use
### R
There is a function named "MRM_finder" in the "R" folder. The function is used to pick ion pairs from ms1 peak detection result and mgf files. And we provided an example which can be seen in the same folder.
#### Parameters of MRM_finder
|Parameters 	|Meaning                                                |
|:--------------|:------------------------------------------------------|
|file_MS1	    |MS1 file (.csv)                                        |
|filepath_MS2   |filepath of MS2 file (.mgf)                            |
|tol_mz         |m/z tolerance between MS1 and MS2 files                |
|tol_rt	        |retention time tolerance between MS1 and MS2 files     |
|diff_MS2MS1	|smallest tolerance between precusor and product ion    |
|ms2_intensity  |smallest intensity of product ion                      |
|resultpath     |result(.csv) filepath                                  |

### Matlab
There is a user mannal in "Matlab" folder. 
