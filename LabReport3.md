# Lab Report 3 - Researching Commands  
  
## Command: find
  
## 1.) -name  
Source: [Link](https://adamtheautomator.com/bash-find/)
### Example 1:
Command:  
```
find technical/biomed -name "rr*.txt"
```
Output:
```
technical/biomed/rr166.txt
technical/biomed/rr167.txt
technical/biomed/rr171.txt
technical/biomed/rr172.txt
technical/biomed/rr191.txt
technical/biomed/rr196.txt
technical/biomed/rr37.txt
technical/biomed/rr73.txt
technical/biomed/rr74.txt
```
Explanation: The use of the command **-name** in this example helped find files in technical/biomed that starts with rr and is a .txt file. It is very useful for filtering out unnecessary files.
### Example 2:
Command:
```
find technical -name "ar3*.txt"
```
Output:
```
technical/biomed/ar309.txt
technical/biomed/ar319.txt
technical/biomed/ar321.txt
technical/biomed/ar328.txt
technical/biomed/ar331.txt
technical/biomed/ar383.txt
technical/biomed/ar387.txt
```
Explanation: The use of the command **-name** in this example helped find all files in technical that starts with ar3 and is a .txt file. It is very useful for filtering out unnecessary files.
## 2.) -type d and -type f
Source: [Link](https://adamtheautomator.com/bash-find/)
### Example 1:
Command:
```
find technical -type d
```
Output:
```
technical
technical/911report
technical/biomed
technical/government
technical/government/About_LSC
technical/government/Alcohol_Problems
technical/government/Env_Prot_Agen
technical/government/Gen_Account_Office
technical/government/Media
technical/government/Post_Rate_Comm
technical/plos
```
Explanation: The use of the command **-type d** in this example finds all the directories in technical. This is useful for sorting out directories from files.
### Example 2:
Command:
```
find technical/plos -name "journal*" -type f
```
Output:
```
technical/plos/journal.pbio.0020001.txt
technical/plos/journal.pbio.0020010.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020013.txt
technical/plos/journal.pbio.0020019.txt
technical/plos/journal.pbio.0020028.txt
technical/plos/journal.pbio.0020035.txt
technical/plos/journal.pbio.0020040.txt
technical/plos/journal.pbio.0020042.txt
technical/plos/journal.pbio.0020043.txt
technical/plos/journal.pbio.0020046.txt
technical/plos/journal.pbio.0020047.txt
technical/plos/journal.pbio.0020052.txt
technical/plos/journal.pbio.0020053.txt
technical/plos/journal.pbio.0020054.txt
technical/plos/journal.pbio.0020063.txt
technical/plos/journal.pbio.0020064.txt
technical/plos/journal.pbio.0020067.txt
technical/plos/journal.pbio.0020068.txt
technical/plos/journal.pbio.0020071.txt
technical/plos/journal.pbio.0020073.txt
technical/plos/journal.pbio.0020100.txt
technical/plos/journal.pbio.0020101.txt
technical/plos/journal.pbio.0020105.txt
technical/plos/journal.pbio.0020112.txt
technical/plos/journal.pbio.0020113.txt
technical/plos/journal.pbio.0020116.txt
technical/plos/journal.pbio.0020121.txt
technical/plos/journal.pbio.0020125.txt
technical/plos/journal.pbio.0020127.txt
technical/plos/journal.pbio.0020133.txt
technical/plos/journal.pbio.0020140.txt
technical/plos/journal.pbio.0020145.txt
technical/plos/journal.pbio.0020146.txt
technical/plos/journal.pbio.0020147.txt
technical/plos/journal.pbio.0020148.txt
technical/plos/journal.pbio.0020150.txt
technical/plos/journal.pbio.0020156.txt
technical/plos/journal.pbio.0020161.txt
technical/plos/journal.pbio.0020164.txt
technical/plos/journal.pbio.0020169.txt
technical/plos/journal.pbio.0020172.txt
technical/plos/journal.pbio.0020183.txt
technical/plos/journal.pbio.0020187.txt
technical/plos/journal.pbio.0020190.txt
technical/plos/journal.pbio.0020206.txt
technical/plos/journal.pbio.0020213.txt
technical/plos/journal.pbio.0020214.txt
technical/plos/journal.pbio.0020215.txt
technical/plos/journal.pbio.0020216.txt
technical/plos/journal.pbio.0020223.txt
technical/plos/journal.pbio.0020224.txt
technical/plos/journal.pbio.0020228.txt
technical/plos/journal.pbio.0020232.txt
technical/plos/journal.pbio.0020241.txt
technical/plos/journal.pbio.0020262.txt
technical/plos/journal.pbio.0020263.txt
technical/plos/journal.pbio.0020267.txt
technical/plos/journal.pbio.0020272.txt
technical/plos/journal.pbio.0020276.txt
technical/plos/journal.pbio.0020297.txt
technical/plos/journal.pbio.0020302.txt
technical/plos/journal.pbio.0020306.txt
technical/plos/journal.pbio.0020307.txt
technical/plos/journal.pbio.0020310.txt
technical/plos/journal.pbio.0020311.txt
technical/plos/journal.pbio.0020337.txt
technical/plos/journal.pbio.0020346.txt
technical/plos/journal.pbio.0020347.txt
technical/plos/journal.pbio.0020348.txt
technical/plos/journal.pbio.0020350.txt
technical/plos/journal.pbio.0020353.txt
technical/plos/journal.pbio.0020354.txt
technical/plos/journal.pbio.0020394.txt
technical/plos/journal.pbio.0020400.txt
technical/plos/journal.pbio.0020401.txt
technical/plos/journal.pbio.0020404.txt
technical/plos/journal.pbio.0020406.txt
technical/plos/journal.pbio.0020419.txt
technical/plos/journal.pbio.0020420.txt
technical/plos/journal.pbio.0020430.txt
technical/plos/journal.pbio.0020431.txt
technical/plos/journal.pbio.0020439.txt
technical/plos/journal.pbio.0020440.txt
technical/plos/journal.pbio.0030021.txt
technical/plos/journal.pbio.0030024.txt
technical/plos/journal.pbio.0030032.txt
technical/plos/journal.pbio.0030050.txt
technical/plos/journal.pbio.0030051.txt
technical/plos/journal.pbio.0030056.txt
technical/plos/journal.pbio.0030062.txt
technical/plos/journal.pbio.0030065.txt
technical/plos/journal.pbio.0030076.txt
technical/plos/journal.pbio.0030094.txt
technical/plos/journal.pbio.0030097.txt
technical/plos/journal.pbio.0030102.txt
technical/plos/journal.pbio.0030105.txt
technical/plos/journal.pbio.0030127.txt
technical/plos/journal.pbio.0030129.txt
technical/plos/journal.pbio.0030131.txt
technical/plos/journal.pbio.0030136.txt
technical/plos/journal.pbio.0030137.txt
```
Explanation: The use of the command **-type f** in this example finds all the file types of technical/plos that starts with journal. This is useful for sorting out the files from other types such as directory.
## 3.) -printf
Source: [Link](https://adamtheautomator.com/bash-find/)
### Example 1:
Command:
```
find technical/plos/pmed* -printf "%p %s \n"
```
Output:
```
technical/plos/pmed.0010008.txt 26395 
technical/plos/pmed.0010010.txt 12791 
technical/plos/pmed.0010013.txt 11220 
technical/plos/pmed.0010021.txt 12743 
technical/plos/pmed.0010022.txt 6155
technical/plos/pmed.0010023.txt 3666
technical/plos/pmed.0010024.txt 3644
technical/plos/pmed.0010025.txt 2882
technical/plos/pmed.0010026.txt 6499
technical/plos/pmed.0010028.txt 39840
technical/plos/pmed.0010029.txt 3003
technical/plos/pmed.0010030.txt 3280 
technical/plos/pmed.0010034.txt 8296
technical/plos/pmed.0010036.txt 36005
technical/plos/pmed.0010039.txt 14627 
technical/plos/pmed.0010041.txt 7742
technical/plos/pmed.0010042.txt 10510
technical/plos/pmed.0010045.txt 24902
technical/plos/pmed.0010046.txt 6465 
technical/plos/pmed.0010047.txt 4110
technical/plos/pmed.0010048.txt 4590
technical/plos/pmed.0010049.txt 4135
technical/plos/pmed.0010050.txt 3513
technical/plos/pmed.0010051.txt 8433 
technical/plos/pmed.0010052.txt 16148
technical/plos/pmed.0010056.txt 15878 
technical/plos/pmed.0010058.txt 16479
technical/plos/pmed.0010060.txt 12102
technical/plos/pmed.0010061.txt 7807
technical/plos/pmed.0010062.txt 28513
technical/plos/pmed.0010064.txt 30704
technical/plos/pmed.0010066.txt 24581 
technical/plos/pmed.0010067.txt 2572
technical/plos/pmed.0010068.txt 2793
technical/plos/pmed.0010069.txt 4015
technical/plos/pmed.0010070.txt 4094
technical/plos/pmed.0010071.txt 5565
technical/plos/pmed.0020002.txt 11012 
technical/plos/pmed.0020005.txt 9682
technical/plos/pmed.0020007.txt 11266
technical/plos/pmed.0020009.txt 17517
technical/plos/pmed.0020015.txt 24420 
technical/plos/pmed.0020016.txt 27409
technical/plos/pmed.0020017.txt 12325
technical/plos/pmed.0020018.txt 38176
technical/plos/pmed.0020019.txt 3316 
technical/plos/pmed.0020020.txt 3812
technical/plos/pmed.0020021.txt 2805
technical/plos/pmed.0020022.txt 3005
technical/plos/pmed.0020023.txt 3600
technical/plos/pmed.0020024.txt 2889
technical/plos/pmed.0020027.txt 2390
technical/plos/pmed.0020028.txt 2045
technical/plos/pmed.0020033.txt 9033 
technical/plos/pmed.0020034.txt 20355
technical/plos/pmed.0020035.txt 6101
technical/plos/pmed.0020036.txt 6483
technical/plos/pmed.0020039.txt 13754
technical/plos/pmed.0020040.txt 17728
technical/plos/pmed.0020045.txt 35552 
technical/plos/pmed.0020047.txt 4033
technical/plos/pmed.0020048.txt 1364
technical/plos/pmed.0020050.txt 29053
technical/plos/pmed.0020055.txt 6358
technical/plos/pmed.0020059.txt 36921
technical/plos/pmed.0020060.txt 12504
technical/plos/pmed.0020061.txt 21501
technical/plos/pmed.0020062.txt 11983
technical/plos/pmed.0020065.txt 4007
technical/plos/pmed.0020067.txt 13417
technical/plos/pmed.0020068.txt 16226 
technical/plos/pmed.0020071.txt 10897 
technical/plos/pmed.0020073.txt 43196
technical/plos/pmed.0020074.txt 3074
technical/plos/pmed.0020075.txt 9476
technical/plos/pmed.0020082.txt 1562
technical/plos/pmed.0020085.txt 2508
technical/plos/pmed.0020086.txt 2147
technical/plos/pmed.0020088.txt 6432
technical/plos/pmed.0020090.txt 3477
technical/plos/pmed.0020091.txt 3609
technical/plos/pmed.0020094.txt 3207
technical/plos/pmed.0020098.txt 8387 
technical/plos/pmed.0020099.txt 8641
technical/plos/pmed.0020102.txt 12234 
technical/plos/pmed.0020103.txt 39679
technical/plos/pmed.0020104.txt 6745 
technical/plos/pmed.0020113.txt 3970
technical/plos/pmed.0020114.txt 3680
technical/plos/pmed.0020115.txt 3672
technical/plos/pmed.0020116.txt 3315
technical/plos/pmed.0020117.txt 3471
technical/plos/pmed.0020118.txt 5819
technical/plos/pmed.0020120.txt 1468
technical/plos/pmed.0020123.txt 25483
technical/plos/pmed.0020140.txt 21124 
technical/plos/pmed.0020144.txt 5737
technical/plos/pmed.0020145.txt 2932
technical/plos/pmed.0020146.txt 3867
technical/plos/pmed.0020148.txt 3781
technical/plos/pmed.0020149.txt 3843
technical/plos/pmed.0020150.txt 3794
technical/plos/pmed.0020155.txt 7068
technical/plos/pmed.0020157.txt 1432 
technical/plos/pmed.0020158.txt 5835
technical/plos/pmed.0020160.txt 28650
technical/plos/pmed.0020161.txt 20401
technical/plos/pmed.0020162.txt 27175
technical/plos/pmed.0020180.txt 7880
technical/plos/pmed.0020181.txt 7085
technical/plos/pmed.0020182.txt 35890
technical/plos/pmed.0020187.txt 4898
technical/plos/pmed.0020189.txt 3500
technical/plos/pmed.0020191.txt 893
technical/plos/pmed.0020192.txt 1061
technical/plos/pmed.0020194.txt 5305 
technical/plos/pmed.0020195.txt 3206
technical/plos/pmed.0020196.txt 3861
technical/plos/pmed.0020197.txt 5778
technical/plos/pmed.0020198.txt 4627
technical/plos/pmed.0020200.txt 3931
technical/plos/pmed.0020201.txt 4145 
technical/plos/pmed.0020203.txt 5451
technical/plos/pmed.0020206.txt 15905
technical/plos/pmed.0020208.txt 6675
technical/plos/pmed.0020209.txt 20355 
technical/plos/pmed.0020210.txt 10798
technical/plos/pmed.0020212.txt 15104
technical/plos/pmed.0020216.txt 20267
technical/plos/pmed.0020226.txt 937 
technical/plos/pmed.0020231.txt 8434
technical/plos/pmed.0020232.txt 16230
technical/plos/pmed.0020235.txt 4810
technical/plos/pmed.0020236.txt 4828
technical/plos/pmed.0020237.txt 4068
technical/plos/pmed.0020238.txt 4515
technical/plos/pmed.0020239.txt 5016
technical/plos/pmed.0020242.txt 5149
technical/plos/pmed.0020246.txt 39380
technical/plos/pmed.0020247.txt 12290
technical/plos/pmed.0020249.txt 38174
technical/plos/pmed.0020257.txt 4736 
technical/plos/pmed.0020258.txt 3431
technical/plos/pmed.0020268.txt 4256
technical/plos/pmed.0020272.txt 6542
technical/plos/pmed.0020273.txt 4546
technical/plos/pmed.0020274.txt 3584
technical/plos/pmed.0020275.txt 4146
technical/plos/pmed.0020278.txt 2779
technical/plos/pmed.0020281.txt 2851
```
Explanation: The use of **-printf "%p %s \n"** in this example create directives or “formatters” that define how the search result will look. The **%p** returns the file's exact name, the **%s** returns the file’s size in bytes, and the **\n** creates a new line for the next file. This is useful for seeing certain information about files in technical.
### Example 2:
Command:
```
find technical/plos/pmed* -printf "%p %t \n"
```
Output:
```
technical/plos/pmed.0010008.txt Thu Apr 27 16:08:33.8221024000 2023 
technical/plos/pmed.0010010.txt Thu Apr 27 16:08:33.8245719000 2023 
technical/plos/pmed.0010013.txt Thu Apr 27 16:08:33.8436073000 2023
technical/plos/pmed.0010021.txt Thu Apr 27 16:08:33.8446050000 2023
technical/plos/pmed.0010022.txt Thu Apr 27 16:08:33.8465569000 2023
technical/plos/pmed.0010023.txt Thu Apr 27 16:08:33.8479159000 2023
technical/plos/pmed.0010024.txt Thu Apr 27 16:08:33.8489127000 2023
technical/plos/pmed.0010025.txt Thu Apr 27 16:08:33.8499099000 2023
technical/plos/pmed.0010026.txt Thu Apr 27 16:08:33.8560107000 2023
technical/plos/pmed.0010028.txt Thu Apr 27 16:08:33.8570081000 2023
technical/plos/pmed.0010029.txt Thu Apr 27 16:08:33.8734838000 2023
technical/plos/pmed.0010030.txt Thu Apr 27 16:08:33.8882757000 2023
technical/plos/pmed.0010034.txt Thu Apr 27 16:08:33.8900201000 2023
technical/plos/pmed.0010036.txt Thu Apr 27 16:08:33.8910166000 2023
technical/plos/pmed.0010039.txt Thu Apr 27 16:08:33.8931651000 2023
technical/plos/pmed.0010041.txt Thu Apr 27 16:08:33.8941678000 2023
technical/plos/pmed.0010042.txt Thu Apr 27 16:08:33.9268281000 2023
technical/plos/pmed.0010045.txt Thu Apr 27 16:08:33.9406578000 2023
technical/plos/pmed.0010046.txt Thu Apr 27 16:08:33.9419129000 2023
technical/plos/pmed.0010047.txt Thu Apr 27 16:08:33.9439099000 2023
technical/plos/pmed.0010048.txt Thu Apr 27 16:08:33.9459025000 2023
technical/plos/pmed.0010049.txt Thu Apr 27 16:08:33.9479078000 2023
technical/plos/pmed.0010050.txt Thu Apr 27 16:08:33.9491661000 2023
technical/plos/pmed.0010051.txt Thu Apr 27 16:08:33.9517776000 2023
technical/plos/pmed.0010052.txt Thu Apr 27 16:08:33.9536125000 2023
technical/plos/pmed.0010056.txt Thu Apr 27 16:08:33.9567613000 2023
technical/plos/pmed.0010058.txt Thu Apr 27 16:08:33.9591644000 2023
technical/plos/pmed.0010060.txt Thu Apr 27 16:08:33.9624690000 2023
technical/plos/pmed.0010061.txt Thu Apr 27 16:08:33.9644625000 2023
technical/plos/pmed.0010062.txt Thu Apr 27 16:08:33.9723378000 2023
technical/plos/pmed.0010064.txt Thu Apr 27 16:08:33.9777783000 2023
technical/plos/pmed.0010066.txt Thu Apr 27 16:08:33.9800159000 2023
technical/plos/pmed.0010067.txt Thu Apr 27 16:08:34.0108254000 2023
technical/plos/pmed.0010068.txt Thu Apr 27 16:08:34.0225769000 2023
technical/plos/pmed.0010069.txt Thu Apr 27 16:08:34.0244391000 2023
technical/plos/pmed.0010070.txt Thu Apr 27 16:08:34.0267650000 2023
technical/plos/pmed.0010071.txt Thu Apr 27 16:08:34.0286042000 2023
technical/plos/pmed.0020002.txt Thu Apr 27 16:08:34.0324600000 2023
technical/plos/pmed.0020005.txt Thu Apr 27 16:08:34.0345754000 2023 
technical/plos/pmed.0020007.txt Thu Apr 27 16:08:34.0365698000 2023
technical/plos/pmed.0020009.txt Thu Apr 27 16:08:34.0524174000 2023
technical/plos/pmed.0020015.txt Thu Apr 27 16:08:34.0949884000 2023
technical/plos/pmed.0020016.txt Thu Apr 27 16:08:34.1036358000 2023
technical/plos/pmed.0020017.txt Thu Apr 27 16:08:34.1056282000 2023
technical/plos/pmed.0020018.txt Thu Apr 27 16:08:34.1089560000 2023
technical/plos/pmed.0020019.txt Thu Apr 27 16:08:34.1111042000 2023
technical/plos/pmed.0020020.txt Thu Apr 27 16:08:34.1121016000 2023
technical/plos/pmed.0020021.txt Thu Apr 27 16:08:34.1143156000 2023
technical/plos/pmed.0020022.txt Thu Apr 27 16:08:34.1376084000 2023
technical/plos/pmed.0020023.txt Thu Apr 27 16:08:34.1396873000 2023
technical/plos/pmed.0020024.txt Thu Apr 27 16:08:34.1417178000 2023
technical/plos/pmed.0020027.txt Thu Apr 27 16:08:34.1427142000 2023
technical/plos/pmed.0020028.txt Thu Apr 27 16:08:34.1457866000 2023
technical/plos/pmed.0020033.txt Thu Apr 27 16:08:34.1499901000 2023 
technical/plos/pmed.0020034.txt Thu Apr 27 16:08:34.1521171000 2023
technical/plos/pmed.0020035.txt Thu Apr 27 16:08:34.1554424000 2023
technical/plos/pmed.0020036.txt Thu Apr 27 16:08:34.1574364000 2023
technical/plos/pmed.0020039.txt Thu Apr 27 16:08:34.1777009000 2023
technical/plos/pmed.0020040.txt Thu Apr 27 16:08:34.1792531000 2023
technical/plos/pmed.0020045.txt Thu Apr 27 16:08:34.1826473000 2023
technical/plos/pmed.0020047.txt Thu Apr 27 16:08:34.1846415000 2023
technical/plos/pmed.0020048.txt Thu Apr 27 16:08:34.1889274000 2023
technical/plos/pmed.0020050.txt Thu Apr 27 16:08:34.1909201000 2023
technical/plos/pmed.0020055.txt Thu Apr 27 16:08:34.2024266000 2023
technical/plos/pmed.0020059.txt Thu Apr 27 16:08:34.2149394000 2023
technical/plos/pmed.0020060.txt Thu Apr 27 16:08:34.2246142000 2023
technical/plos/pmed.0020061.txt Thu Apr 27 16:08:34.2274222000 2023
technical/plos/pmed.0020062.txt Thu Apr 27 16:08:34.2294163000 2023
technical/plos/pmed.0020065.txt Thu Apr 27 16:08:34.2320332000 2023
technical/plos/pmed.0020067.txt Thu Apr 27 16:08:34.2378976000 2023
technical/plos/pmed.0020068.txt Thu Apr 27 16:08:34.2400509000 2023
technical/plos/pmed.0020071.txt Thu Apr 27 16:08:34.2422532000 2023
technical/plos/pmed.0020073.txt Thu Apr 27 16:08:34.2466993000 2023
technical/plos/pmed.0020074.txt Thu Apr 27 16:08:34.2513355000 2023
technical/plos/pmed.0020075.txt Thu Apr 27 16:08:34.2534949000 2023
technical/plos/pmed.0020082.txt Thu Apr 27 16:08:34.2550637000 2023
technical/plos/pmed.0020085.txt Thu Apr 27 16:08:34.2596582000 2023
technical/plos/pmed.0020086.txt Thu Apr 27 16:08:34.2701228000 2023
technical/plos/pmed.0020088.txt Thu Apr 27 16:08:34.2721153000 2023
technical/plos/pmed.0020090.txt Thu Apr 27 16:08:34.2737524000 2023
technical/plos/pmed.0020091.txt Thu Apr 27 16:08:34.2802401000 2023
technical/plos/pmed.0020094.txt Thu Apr 27 16:08:34.2836101000 2023
technical/plos/pmed.0020098.txt Thu Apr 27 16:08:34.2849413000 2023
technical/plos/pmed.0020099.txt Thu Apr 27 16:08:34.2876342000 2023
technical/plos/pmed.0020102.txt Thu Apr 27 16:08:34.2896274000 2023
technical/plos/pmed.0020103.txt Thu Apr 27 16:08:34.2936607000 2023
technical/plos/pmed.0020104.txt Thu Apr 27 16:08:34.2962991000 2023
technical/plos/pmed.0020113.txt Thu Apr 27 16:08:34.2982944000 2023
technical/plos/pmed.0020114.txt Thu Apr 27 16:08:34.2992894000 2023
technical/plos/pmed.0020115.txt Thu Apr 27 16:08:34.3019417000 2023
technical/plos/pmed.0020116.txt Thu Apr 27 16:08:34.3037959000 2023
technical/plos/pmed.0020117.txt Thu Apr 27 16:08:34.3054243000 2023
technical/plos/pmed.0020118.txt Thu Apr 27 16:08:34.3074171000 2023
technical/plos/pmed.0020120.txt Thu Apr 27 16:08:34.3094111000 2023 
technical/plos/pmed.0020123.txt Thu Apr 27 16:08:34.3114815000 2023
technical/plos/pmed.0020140.txt Thu Apr 27 16:08:34.3127324000 2023
technical/plos/pmed.0020144.txt Thu Apr 27 16:08:34.3137304000 2023
technical/plos/pmed.0020145.txt Thu Apr 27 16:08:34.3349613000 2023
technical/plos/pmed.0020146.txt Thu Apr 27 16:08:34.3368461000 2023
technical/plos/pmed.0020148.txt Thu Apr 27 16:08:34.3523215000 2023
technical/plos/pmed.0020149.txt Thu Apr 27 16:08:34.3534370000 2023
technical/plos/pmed.0020150.txt Thu Apr 27 16:08:34.3646063000 2023
technical/plos/pmed.0020155.txt Thu Apr 27 16:08:34.3667130000 2023
technical/plos/pmed.0020157.txt Thu Apr 27 16:08:34.3677104000 2023
technical/plos/pmed.0020158.txt Thu Apr 27 16:08:34.3687087000 2023
technical/plos/pmed.0020160.txt Thu Apr 27 16:08:34.3708493000 2023
technical/plos/pmed.0020161.txt Thu Apr 27 16:08:34.3729285000 2023
technical/plos/pmed.0020162.txt Thu Apr 27 16:08:34.3749609000 2023
technical/plos/pmed.0020180.txt Thu Apr 27 16:08:34.3763922000 2023
technical/plos/pmed.0020181.txt Thu Apr 27 16:08:34.3773895000 2023
technical/plos/pmed.0020182.txt Thu Apr 27 16:08:34.3793837000 2023
technical/plos/pmed.0020187.txt Thu Apr 27 16:08:34.3814607000 2023
technical/plos/pmed.0020189.txt Thu Apr 27 16:08:34.3832026000 2023
technical/plos/pmed.0020191.txt Thu Apr 27 16:08:34.3843847000 2023
technical/plos/pmed.0020192.txt Thu Apr 27 16:08:34.3853826000 2023
technical/plos/pmed.0020194.txt Thu Apr 27 16:08:34.3869804000 2023
technical/plos/pmed.0020195.txt Thu Apr 27 16:08:34.3882537000 2023
technical/plos/pmed.0020196.txt Thu Apr 27 16:08:34.3897723000 2023
technical/plos/pmed.0020197.txt Thu Apr 27 16:08:34.3907691000 2023
technical/plos/pmed.0020198.txt Thu Apr 27 16:08:34.3927640000 2023
technical/plos/pmed.0020200.txt Thu Apr 27 16:08:34.3947591000 2023
technical/plos/pmed.0020201.txt Thu Apr 27 16:08:34.3958638000 2023
technical/plos/pmed.0020203.txt Thu Apr 27 16:08:34.3968614000 2023
technical/plos/pmed.0020206.txt Thu Apr 27 16:08:34.3978590000 2023
technical/plos/pmed.0020208.txt Thu Apr 27 16:08:34.3990341000 2023
technical/plos/pmed.0020209.txt Thu Apr 27 16:08:34.4010292000 2023
technical/plos/pmed.0020210.txt Thu Apr 27 16:08:34.4020252000 2023
technical/plos/pmed.0020212.txt Thu Apr 27 16:08:34.4246475000 2023
technical/plos/pmed.0020216.txt Thu Apr 27 16:08:34.4256448000 2023
technical/plos/pmed.0020226.txt Thu Apr 27 16:08:34.4266420000 2023
technical/plos/pmed.0020231.txt Thu Apr 27 16:08:34.4276395000 2023
technical/plos/pmed.0020232.txt Thu Apr 27 16:08:34.4286363000 2023
technical/plos/pmed.0020235.txt Thu Apr 27 16:08:34.4296342000 2023
technical/plos/pmed.0020236.txt Thu Apr 27 16:08:34.4305930000 2023
technical/plos/pmed.0020237.txt Thu Apr 27 16:08:34.4305930000 2023
technical/plos/pmed.0020238.txt Thu Apr 27 16:08:34.4325870000 2023
technical/plos/pmed.0020239.txt Thu Apr 27 16:08:34.4338878000 2023
technical/plos/pmed.0020242.txt Thu Apr 27 16:08:34.4339854000 2023
technical/plos/pmed.0020246.txt Thu Apr 27 16:08:34.4377622000 2023
technical/plos/pmed.0020247.txt Thu Apr 27 16:08:34.4423454000 2023
technical/plos/pmed.0020249.txt Thu Apr 27 16:08:34.4440612000 2023
technical/plos/pmed.0020257.txt Thu Apr 27 16:08:34.4448487000 2023
technical/plos/pmed.0020258.txt Thu Apr 27 16:08:34.4448487000 2023
technical/plos/pmed.0020268.txt Thu Apr 27 16:08:34.4460758000 2023
technical/plos/pmed.0020272.txt Thu Apr 27 16:08:34.4901306000 2023
technical/plos/pmed.0020273.txt Thu Apr 27 16:08:34.4911276000 2023 
technical/plos/pmed.0020274.txt Thu Apr 27 16:08:34.4911276000 2023
technical/plos/pmed.0020275.txt Thu Apr 27 16:08:34.4921257000 2023
technical/plos/pmed.0020278.txt Thu Apr 27 16:08:34.4931220000 2023
technical/plos/pmed.0020281.txt Thu Apr 27 16:08:34.4945378000 2023
```
Explanation:The use of **-printf "%p %s \n"** in this example create directives or “formatters” that define how the search result will look. The **%p** returns the file's exact name, the **%t** returns the file’s last modification time, and the **\n** creates a new line for the next file. This is useful for seeing certain information for files in technical.
## 4.) -exec
Source: [Link](https://adamtheautomator.com/bash-find/)
### Example 1:
Command:
```
find technical/plos -name "pmed.0020281.txt" -exec rm -i {} \;
```
Output:
```
rm: remove regular file 'technical/plos/pmed.0020281.txt'?
```
Explanation: The use of the command **-exec rm -i {} \;** in this example removed the file pmed.0020281.txt. This feature is very useful for deleting certain files if you know the names of them. It is also different from a regular rm as it will asks for user confirmation before deleting each file. This ensures that you avoid accidentally removing files, especially when dealing with multiple files.
### Example 2:
Command:
```
find technical/plos -name "journal.pbio.0030137.txt" -exec vi -i {} \;
```
Output:
```

~
~                                                          VIM - Vi IMproved
~
~                                                          version 9.0.1302
~                                                      by Bram Moolenaar et al.
~                                             Vim is open source and freely distributable
~
~                                                    Become a registered Vim user!
~                                           type  :help register<Enter>   for information 
~
~                                           type  :q<Enter>               to exit
~                                           type  :help<Enter>  or  <F1>  for on-line help
~                                           type  :help version9<Enter>   for version info
~
~
[No Name] [unix] (15:59 31/12/1969)                                                                           
```
Explanation: The use of the command **-exec vi -i {} \;** opens up the file in a text editor called vim. This is very useful for if you want to edit a file or view it on a different screen. This also allows you to edit a code file without having to open it up on a new workspace.
