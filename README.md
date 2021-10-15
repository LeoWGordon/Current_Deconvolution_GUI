# Current_Deconvolution_GUI

README for Current_Deconvolution_GUI [1]
Latest Version: 3.2.3 - 15th October 2021 

This GUI will take variable rate cyclic voltammetry (CV) data (at least 3 rates) and deconvolute the current using the methods described in Wang et al. [2].

First use the "Format Data" tab to open an auxilliary GUI which formats the CV data to be processed by the GUI. The formatting GUI can either format a single file which contains all rates, or can concatenate multiple files together to create a single 'variable-rate' spreadsheet, in this case the files must all have the same format (same headers, same sheet number).
This file will have the name "Formatted_multiple_input.txt" and will save in the folder that the original data came from.
If variable-rate data was acquired in a single file via the EC-Lab software, the data should already be in the correct format for processing.

Once the formatted data file is ready, navigate to the "Load Data" tab, and click "Browse Data" to open the file explorer where the formatted data file can be selected.
The selected file name will populate the text box (default is "Data File"), then click "Load Formatted Data". 
The data will plot in the in-built axes, if the data contained multiple cycles for each rate, the last cycle will be chosen.
The voltage limits can be edited at any time. The table in the bottom-left will be populated with different rates present in the input data, and can be selected and de-selected as required - this will reflect in the plot in the in-built axes.
The drop-down box below allows the user to select which rate to plot the deconvolution analysis onto.

The variable rate CV axes are able to recieve mouse-click inputs to select a window to be designated as a region of true capacitance, for use of decoupling double-layer capacitance from pseudocapacitance. The region can be selected for either oxidation or reduction sweep and must be indicated by the button in the top-right corner, which will indicate which sweep is being used via the word "Oxidation" or "Reduction".

After the rate to be deconvoluted, the cycles to be used for the deconvolution, and the region of true capacitance have been selected, the "Deconvolute Current" button should be clicked, which will create a figure of the deconvoluted data. The "Save Deconvoluted Current Plot" text box can be edited for a desired file name, and file type should be chosen from the drop-down menu, before clicking the "Save Figure" button.

For a table of the deconvoluted currents and decoupled capacitance/pseudocapacitance, click "Get Table". An Excel spreadsheet will be created and saved to the same folder as the input data.

For any further queries or feedback, please contact me at lgordon@ccny.cuny.edu

[1] Under review: T. Schoetz, L. W. Gordon, S. Ivanov, A. Bund, D. Mandler,* and R. J. Messinger
Disentangling Charge Storage Mechanisms in Hybrid Energy Storage Systems: 
A Tutorial for the Characterization of Batteries and Capacitors
[2] Wang, J., Polleux, J., Lim, J. & Dunn, B. Pseudocapacitive Contributions 
to Electrochemical Energy Storage in TiO 2 (Anatase) Nanoparticles. 
J. Phys. Chem. C 111, 14925–14931 (2007).
