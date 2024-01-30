NMR pulse sequences and RF shapes for the experiments reported in Manu, et.al. ChemmComm (2024)

Cite Reference articles @ Manu, et.al. ChemmComm (2024)

The script and algorithms are patented @ https://patentcenter.uspto.gov/#!/applications/16861506


 
experimental setup in a bruker Spectrometer:
1.Copy the the pulse program 'rapidhmqc.mpp' to any of the Bruker pulse program path. And copy pulse shapes (*.mrf) to the Bruker wave directory.
2. Create a new 2D experiment.
3. Enter the following topspin commands. (Adjust the values if required)

"rpar FHSQCF3GPPH all"
"pulprog rapidhmqc.mpp"
"o3p 118"
"1 sw 36"
"spnam25 z2iyAz2z120xA0.9cs_rf0.00_31.977p1_bw0.00p1.mrf"
"spnam26 BandSelRe4_rf0.00_28.400p1_bw0.00p1.mrf" 
"p62 50"
"d1 0.2"
"ds 16"
"ns 2"
"rg 203"
"1 td 128"
"2 td 1024"
"cnst4 95"

Here p62 is a selectivity parameter. Increase the number to ~100 to observe peaks very close to water -- However this decreases the total bandwidth. 


Copyright & License Statement

RF pulse shapes are copyrighted by Regents of the University of Minnesota and the software for generating RF shapes covered by US patent 11,221,384. Regents of the University of Minnesota will license the use of RF shapes solely for educational and research purposes by non-profit institutions and US government agencies only. For other proposed uses, contact umotc@umn.edu. The software may not be sold or redistributed without prior approval. One may make copies of the software for their use provided that the copies, are not sold or distributed, are used under the same terms and conditions. As unestablished research software, this code is provided on an "as is'' basis without warranty of any kind, either expressed or implied. The downloading, or executing any part of this software constitutes an implicit agreement to these terms. These terms and conditions are subject to change at any time without prior notice.

