# Altium Designer templates with Euro Circuits design rules

Since the beginning of 2024 EuroCircuits decided to remove Altium templates and scripts from the website, this repo serves as a backup for those files.

Files were downloaded from Euro Circuits on 19/dez/2023

# The webpage went as follows:

Altium Designer Templates (PcbDoc) help to check your layout against the Eurocircuits technology classification (6C and 8D). This way you can easily define which Eurocircuits service is most suited for your board, and avoid documentation problems after you place your order.

## There are 8 PcbDoc”s :
### Classification for PCB proto and Standard pool:

Class 6C – 2 layer – 1.55 mm

Class 6C – 4 layer – 1.55 mm

Class 6C – 6 layer – 1.55 mm

Class 6C – 8 layer – 1.55 mm

### Classification for Tech pool:

Class 8D – 2 layer – 1.55 mm

Class 8D – 4 layer – 1.55 mm

Class 8D – 6 layer – 1.55 mm

Class 8D – 8 layer – 1.55 mm


There are also 2 scripts available to check the annular ring of your design

The “FindAnnularRing_XX.pas” script is capable to check the annular ring for OAR and
IAR on the appropriate values for PTH (PHD is finished hole size + 100µm).

FindAnnularRing_6C.pas:Altium Designer Rule script for checking onPattern Class 6C,
FindAnnularRing_8D.pas:Altium Designer Rule script for checking onPattern Class 8D,


## How to use this package:

Select the required Pattern / Drill class (6C of 8D) and number of layers.

Put a copy of the PcbDoc in your Altium Designer project folder (*.PcbPrj).

Put a copy of the script (6C or 8D) in your project folder.

From this moment the EuroCircuits rules for Pattern Class, Drill Class and layer-stack is available in the design.

## Remarks:
The minimum annular ring rule “Minimum-IAR” is set to the IAR value of the Pattern class. This value is larger than the OAR. When “Top-Middle-Bottom” or “Full stack” is used it is possible to change the OAR to the (smaller) values of the Pattern Class.

Altium Designer checks the minimal annular ring value when “Top-Middle-Bottom” or “Full stack” is used the OAR can be set smaller than the IAR. The“FindAnnularRing_XX.pas” script is capable to check the annular ring for OAR and IAR on the appropriate values for PTH (PHD is finished hole size + 100µm).

## Disclaimer: 
The *.PcbDoc and *.Pas files are provided by Transfer B.V. “as is”. The use of the documents is at your own risk, no rights to the use of these documents are derived.

Any comments, corrections or additions are appreciated and can be sent to euro@eurocircuits.com

