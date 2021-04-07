# metagenomics_guidlines
Helpful tips for designing metagenomics experiments

Shotgun metagenomics

## Read length
For shotgun metagenomics data, two available lengths are 150 bp and 250 bp. To see if there is a difference between the two, one a dataset of mouse samples, we tested if read length made a difference. To test this, we shortend our orginal reads of length 250 bp to either close to 150 by removing 100 (250-150 =100) bps or by fixing the legnth to 150 bp using cutadapt. 

In these samples, we found that with longer reads 2 more bacterial species (Eggerthella_lenta, Enterococcus_faecalis) were annotated with read length 250bp. A viral species was also identified.


## Sequencing depth
For checking if sequencing depth makes a difference in identifying species, we would recommend reading this paper https://msystems.asm.org/content/3/6/e00069-18

In our test,for 100 samples + mock samples, with 3 M reads (shallow) or 9 M reads (deep) very minor differences were found. All samples corrrelated very well with when compared at 2 different depths (mean=0.993,df=0.03). In deep sequencing samples, we found that 73 species were annotated more than shallow sequencing. However for most of the species relative abundance values in deep samples were < 1e-4 except for Achromobacter_ruhlandii, a species present in our mock samples which was not identified with shallow sequencing.

## Percent annotated

In our expericence, with using the commonly used annotation packages like metaphlan3, kraken2 or Kaiju on average 47.6 % (sd=12.89,n=210) of the reads can be unclassfied. 

