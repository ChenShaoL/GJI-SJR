#GJI-SJR
#Source code and model files for three cases in GJI

#The file contains two parts: source code and ANSYS model. Firstly, generate the finite element model in ANSYS and export the Nlist.dat and Elist.dat files. Use the code in 'preprocess' for preprocessing to generate NODE, BOUND, and Element. Subsequently, use the code in 'freefield' to calculate the free field response, and finally use the code in 'ssi' to start 2D/3D finite element calculation.

#Note: Before using the code, it is necessary to modify the parameters in each preparation file. In the preprocessing section, it is necessary to modify the element/node/model size/element size in PRE.F90. In the free field section, it is necessary to modify information such as material density, wave velocity, and model size in the DAT file. In the SSI section, it is necessary to modify the corresponding parameters in the COMD3.F90 and DS.DAT files. The artificial wave velocity of transmitting boundary and material parameters are contained in DS.DAT. COMD3.F90 includes file paths, number of element/node/boundary node, material types, etc.
