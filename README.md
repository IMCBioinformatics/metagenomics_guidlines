# metagenomics_guidlines
Helpful tips for designing metagenomics experiments

Shotgun metagenomics

## Read length
For shotgun metagenomics data, two available lengths are 150 bp and 250 bp. To see if there is a difference between the two, one a dataset of mouse samples, we tested if read length made a difference. To test this, we shortend our orginal reads of length 250 bp to either close to 150 by removing 100 (250-150 =100) bps or by fixing the legnth to 150 bp using cutadapt. 

In these samples, we found that with longer reads 3 extra species were annotated but only one had relative abundance values > 1e-4.



## Sequencing depth
For checking if sequencing depth makes a difference in identifying species, we would recommend reading this paper https://msystems.asm.org/content/3/6/e00069-18


## Percent annotated

