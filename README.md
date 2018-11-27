### Purpose: this algorithm calculates peak area for each peptide type (you designate) i.e. all species of H3K9 methylation in a sample then outputs individual replicates peak area. It then averages and provides standard deviation of all replicates in the same sample_group for groups of up to 3 technical/biological replicates for each peptide species i.e. H3K9me1. Furthermore, it is extensible to new modifications if you mark them in the peptide note  


Input format: you must export your file to have this format from skyline as a .tsv


Library Peptides		#N/A	#N/A	TKQTAR	T[+119]K[+56]QTAR	440.237784	2	ddcc-0-1.raw	14747159552	13504712704	16763347	1242446080	precursor	8498734080	0	K4un

known possible errors:

error1: if you get an Index traceback error there may be space at the end of your outputfile.tsv, remove it...
error2: adding samples that aren't present in your dataset causes errors similar to this: File "Automating_MSMS_calculations.py", line 114, in aggreg2   

