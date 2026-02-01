<h1>Post-Processing FLUKA Output</h1>

The attached files enable post-processing of FLUKA energy-deposition and DPA output using Python. This approach provides greater flexibility than the built-in FLAIR post-processing tools and allows for manipulating 1D and 2D data across detectors. Before running the Jupyter notebooks, ensure the required libraries are installed. For specific guidance on input file format, see notebook comments. 

<h3>Required Libraries:</h3>

- matplotlib
- numpy
- scipy
- pandas

<h2>Included Functionality</h2>

<h3>DPA Processing</h3>

The _dpa.ipynb_ file allows plotting Norgett-Robinson-Torrens (NRT) and athermal recombination-corrected (ARC) DPA estimates side by side for further comparison. This code can be used to manipulate 1D FLUKA data for any other USERBIN scoring, if desired. 

<img width="4399" height="1209" alt="DPA_Max_Tungsten" src="https://github.com/user-attachments/assets/81567766-7597-4c83-a51d-4b505b78d2ca" />

<h3>Energy Deposition to CSV</h3>

The file named _endep_to_csv.ipynb_ contains code necessary to transform FLUKA output, given in the software-specific format, into a .csv file for further use in ANSYS or equivalent engineering software. The code works for X-Y-Z and R-Ф-Z binning, with output columns including the corresponding bin coordinates, maximum and average power delivered in the bin, and the percentage error in those values. 

<h3>Energy Deposition Histograms</h3>

With _endep.ipynb_, one can transform complex FLUKA energy deposition data into histograms with separated contributions by distinct particle species. The code is specifically designed to manipulate contributions by protons, beam protons, photons, neutrons, electrons, light ions (deuteron, triton, helium-3, and helium-4), and heavy ions. The examples of produced histograms include: 

<img width="3669" height="2149" alt="Tungsten_TotalEn" src="https://github.com/user-attachments/assets/9e8e48d0-6a6c-48e6-aa9c-85bf2a1bc170" />

<img width="3649" height="1687" alt="Tungsten_Protons" src="https://github.com/user-attachments/assets/43c22a27-29fc-41f1-859e-f3600e329e04" />

<img width="3649" height="1687" alt="Tungsten_AllIons" src="https://github.com/user-attachments/assets/fa0de7a8-e3fc-4320-b44c-5dcb61ce090f" />



