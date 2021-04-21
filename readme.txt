This text is an introduction about the intermediate calculation files of the GRL manuscript "Origin of Electron Boomerang Stripes: Statistical Study".
It include 86 "Boomerang-shaped" stripe events and 27 straight stripe events observed by two Van Allen Probes from 2013/01/01 to 2017/12/31.
---------------------
As for a "boomerang-shaped" event happened at "hhmm(UT)" on "yyyy/mm/dd", one can find the relavent files in the zip file: "Boomerang_rbspX_yyyy.zip"(X can be A or B).
These files are a figure about the case (containing electron residual flux on energy spectrum and on pitch angle spectrum of some notable energy channels), 
a figure about the traceback origins compared with plasmapause (from PTP simulation, more details can be found in the acknowledgement),
a txt about the L shells and MLTs of the traceback origins, and a txt about the mean plume range and the distance between the plume and traceback origins.
---------------
Figure A: "Boomerang_rbspX__yyyymmdd_ut_hhmm.pdf"("X" can be "A" or "B", on behalf of the satellite.)
--------
Figure B: "Plasmapause_and_origin_of_boomerang_yyyymmdd_ut_hhmm.pdf"(only from 2013/01/01 to 2015/08/31)
--------
Text A:"Tracebacks_yyyymmdd_ut_hhmm.txt"
In text A, it contains the following parts.
yyyymmdd hhmm
energy1(keV)    ;which energy channel do we calculate the traceback origins?
L_shell1     MLT1
L_shell2     MLT2
…
L_shelln     MLTn     ;corresponding to the traceback circles in Figure 2c
energy2(keV)
…
---------
Text B: "Plasmapause_yyyymmdd_ut_hhmm.txt"
In text B, it contains the following parts.
0 or 1; 0 means there is no plume, otherwise 1.
L_shell_mean
MLT_mean ;The average value of the traceback Lshells and MLTs in Text A, corresponding to Figure 2d
MLT_deviation ;The standard deviation of MLT in Text A.
MLT_width ; the width of the plume on the L_shell_mean
MLT_centre ; the centre of the plume on the L_shell_mean
η ; (MLT_mean-MLT_centre)/MLT_width, as equation (3) in the manuscript
dη ; MLT_deviation/MLT_width, corresponding to the error bar in Figure 4

---------------------
As for a straight stripe event, the files are simular to these of a "boomerang-shaped" one but without traceback origins. One can find them in the zip file: "Straight_rbspX"/"Plasmapause_straight".
----------
Figure A: "Straight_rbspX_yyyymmdd_ut_hhmm.pdf";electron residual flux in a straight stripe event
Figure B: "rbspX_palsmapause_and_straight_yyyymmdd_hhmm.pdf"; plasmapause and the orbit of the satellite
Text A: "rbspX_plasampause_and_straight_yyyymmdd_ut_hhmm.txt"
In text A, it contains the following parts.
X(A or B) yyyymmdd hhmm(UT) energy
L_mean(satellite) MLT_mean(satellite) MLT_middle(plume) MLT_width(plume)
