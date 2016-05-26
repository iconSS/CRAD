# CRAD: a matlab program for preprocessing LC-MS datasets.
The program is capable of batch processing. The number of samples is within the range from 1 to 1000.
The number of LC separation conditions is within the range from 1 to 1000.
The raw datasets of LC-MS includes: LC-UV spectra, which should be saved in txt file, the name of such file is SamXXConYY.txt;
LC-MS spectra which should be saved in matlab file, the name of such file is SamXXConYYP.mat or SamXXConYYN.mat. 
Here the "P" or "N" indicate the ionization mode in positive mode or negative mode. "XX" indicates the sample ID and "YY" indicates condition ID;
The Mobile_Phase.txt file, which includes all the gradients adopted in the LC-MS elutions. 
Generally, the gradient enabled the fasted elution of all the compounds is numbered as the first gradient.

After processing, the TICSSamXXConYYP.txt or TICSSamXXConYYN.txt generated in the root folder can be plotted as the raw TIC and preprocessed TIC.
The XICSSamXXConYYP.txt or XICSSamXXConYYN.txt generated in the root folder can be plotted as the deconvolved XICs.
The MASSSamXXConYYP.txt or MASSSamXXConYYN.txt generated in the root folder list the m/z values of all the deconvlved XICs.

The in-depth clustering results is saved in the subfolder named as "IDC_HILIC_SamXX".
Typically, the data files inside includes "IDCSSamXXN.txt" and "IDCSSamXXP.txt".
In the data file, the first three column data indicates the retention behavior of ions in such bin. 
The fourth column data indicates the retention time of such bin under gradient 1.
The fifth and sixth column data indicates the isotope ratio and relative intensity.
After the sixth column, the m/z values of ions are listed.



