# gcj-dataset-c_cpp-ELF_PE
Extracted C and CPP source code from GCJ dataset 2008 to 2020 and then compiled as ELF and PE binaries for use in "Authorship Attribution for Cyber Security using Machine Learning" paper

Manual steps to extract the code:
Filter col G (file) by "contains .c" which will include .c, .cpp, and .cc
Filter col B (year) for those not matching the year part of the file name (gcjYEAR.csv)
filter col I (flines/code) for blanks
copy visible cells and paste in a new Excel file gcjYEAR.xlsx
find/replace ï»¿ (erroneous part of code usually appearing on the first line)
row height = 15 for readability
enter formula "=TEXTJOIN("_",TRUE,B2,A2,C2,D2,E2)" in cell J2 and fill down (file naming convention)
copy column J and "paste as value" into column A
delete column J
