# RawVegetable 2.0
A quality control software with specialized modules for XLMS experiments. RawVegetable 1.0 can be found at http://patternlabforproteomics.org/rawvegetable/

_<b>Please cite our paper:</b>_<br/>
_Kurt, LU, et al., [“RawVegetable 2.0: Refining XL-MS Data Acquisition through Enhanced Quality Control”](https://doi.org/10.1021/acs.jproteome.3c00791), Journal of Proteome Research, 2024._

# Equipment
## Hardware
A computer with a minimum of 16 GB RAM and 4 computing cores is recommended. However, the software can take advantage of superior configurations.
## Software
- Windows 10 (64 bits) or later.
- The .NET Core 6 or later, which can be downloaded at https://dotnet.microsoft.com/en-us/download/dotnet/6.0
- The RawVegetable software, available for download at https://github.com/loukurt/RawVegetable2/releases

# Tutorial
## Loading Spectra Files
-	Spectra data can be loaded from files in the *.raw, *.mzML, *.ms1 or *.mgf formats, by either dropping them on the main screen or by clicking at **File** and then **Load Files**. Multiple files can be loaded at the same time. (Note: for *.ms1 files, RawVegetable will attempt to find the respective *.ms2 file necessary for some modules, if it cannot be found, the features will be disabled. The same will happen for *.mgf if it only contains MS1 spectra)

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/91b8c8b5-6210-48f2-ba66-b69d8c0ba99e" width="650"><br/>
<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/8b0012c6-c8a8-4ac3-8fb5-f9d19b59a25c" width="650"><br/>

## Loading Identification Files
- For some of the modules, it may be necessary to load an identification file (either of linear or cross-linked peptides). To do this, go to the **File** menu, and click on the **Load ID Files** button.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/3af3f545-094b-48e3-b54b-b4a93493965e" width="650"><br/>
	
- RawVegetable 2.0 only accepts identification files in the form of tables in the *.csv or *.txt formats.
- Once the file has been selected, the software will ask for the column splitter (whether it is a comma or tab-separated) and whether the file contains a header row.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/a8c643bd-ea6e-42fd-b3af-415ec3d0e9cf" width="650"><br/>

- Once this is informed, click the button **Ok**.
- A screen asking you to provide information about the columns will appear. There, it is possible to create a new template (by clicking the button **Add New**) and fill all information prompted, such as which columns are the sequence, m/z, charge, and the other parameters. Note that not all information is necessary for all analyses (and for example, if the m/z and charge are provided, the MH is not necessary and so on), but try to fill as much as possible.
- Once the new template is complete, it is possible to save this library, so it will not be necessary to fill this information again.
- Before closing the window, select your template on the right side of the screen so your ID file can be correctly read.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/3a2654b4-5b80-4802-871f-bfb69a95d4ce" width="650"><br/>

## Navigating Open Files

- The user has full control of which files should be displayed in the screen and used for specific modules by opening the **Open Files** menu once the files have loaded and (un)checking the specific files/plots.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/3184857c-4564-4d5f-bc89-cf52d84474c7" width="650"><br/>

- It’s also possible to change the colours used for each file by right-clicking on the name of the file.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/5a63c103-5c42-46f3-a944-0ce99c8315b9" width="650"><br/>

## Chromatograms

-	Once the files have finished loading, the chromatograms will be shown on the screen as shown below.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/b245aa06-2a9d-4ea9-a6f1-49c0d95702af" width="650"><br/>

- The chromatograms can also be viewed separately by clicking in **Graphical Options** and then **Separated by File**.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/d94f8395-3bcc-43e7-923f-59aa4e02f5fb" width="650"><br/>

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/09867ae2-fcd7-48d7-95de-82be88b1b53e" width="650"><br/>

- It’s possible to change the type of chromatogram from TIC to Base Peak Only by going on the **Open Files** menu, right-clicking on the specific file then on **Chromatography -> Base Peak Only**.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/016556f6-6c7b-47a1-80cf-412dadd41d37" width="650"><br/>

## Charged Chromatogram

- In order to see the charge-specific chromatograms, go to the **Analysis** menu and click on the **Deconvolute** button. This process will deconvolute all the files that are checked in the **Open Files** menu and can take minutes to conclude according to the size of the files.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/2ebaa7ca-ec10-4534-8197-06336f1cc59b" width="650"><br/>

- Once the deconvolution is complete, select the charge you want to view on the **Open Files** menu. You can identify the chromatograms by clicking on it or by changing their colours on the **Open Files** menu (right-click on the specific charge).

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/2bab40ef-1cbf-46a0-9cb6-5525aeada36b" width="650"><br/>

- If you want to see more than one charge as a single chromatogram, select the charges on the combo box shown below and click the **Merge** Button. The merged chromatogram will now be shown on the **Open Files** menu.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/60696748-e031-4d68-a9fd-05cd690c3d97" width="650"><br/>

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/daeea76e-e99c-4c13-9a04-993da8b71ed2" width="650"><br/>

## TopN Density Estimation

- In order to check TopN Density Estimation of the loaded files, go to the **TopN** tab, and to the **TopN** menu for further options.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/af45c8ce-2b79-445a-92e0-d8ed50ce4c52" width="650"><br/>

- In the **TopN** menu it’s possible to change the standard deviation used for the gaussian function in this module. There, it’s also possible to select a single precursor charge to build the density estimation based only on those specific spectra by choosing a charge and clicking on **Plot**. 

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/533df454-b75f-4e4e-ab24-adb88b68575b" width="650"><br/>

- Once the density estimation has been calculated, the curve will appear on the TopN viewer and you can view/hide it by clicking on the checkbox under the TopN item for each file on the **Open Files** menu.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/43ded518-0962-4af5-b639-a1b272678eef" width="650"><br/>

- A boxplot showing the distribution of MS2 scans by MS1 can also be seen by clicking on the **Box Plots** menu on the left side of the **TopN Viewer**.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/da238bb0-39c9-4c17-be4a-e74ac8baebae" width="650"><br/>

## Precursor Signal Ratio

- To check the Precursor Signal Ratio distribution of the loaded files, you can click on the **Precursor Signal Ratio** tab.
- In this viewer, it’s possible to change the number of bins, as well as maximums and minimums for the histogram.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/30fd74a7-edbc-41cf-9036-274dc953555d" width="650"><br/>

## Xrea

- For the Xrea plots, click on the **Xrea** tab once the files have been loaded.
- Here it’s possible to adjust the parameters for the smoothing algorithm used (Savitzky-Golay).

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/d14ed9db-2741-44a9-8636-c1b555daabe9" width="650"><br/>

- The light-coloured lines are the actual Xrea values per MS2 scan, while the dark-coloured one are the smoothed lines. You may hide either one by going on the **Open File** menu and (un)checking them.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/108a8a1a-7f97-4d54-8271-778f46728db8" width="650"><br/>

## Pair Finder

- To run the Pair Finder module, go to the **Pair Finder** menu. There, some parameters must be set before clicking on **Run**. The results will appear on the **Pair Finder** tab.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/ad7b59c0-5a5c-492b-8bf4-f64697b0537e" width="650"><br/>

- The necessary parameters are as follows:
	- **Pair Search PPM**: the ppm tolerance allowed for the m/z of the pair’s peaks. Default is 20.
	- **Full Pairs Only**: if this option is checked, the algorithm will only consider a true doublet if all four peaks are present. If it’s unchecked, three peaks are enough. Default is unchecked.
	- **Intensity Threshold**: the cut-off ratio for the intensity where a peak is considered noise. This value is relative to the maximum of the spectrum; for example, if you set this parameter as 0.01, peaks with intensity lower than 1% of the highest peak of the spectrum will be considered noise. Default is 0.
	- **Max. Charges**: the number of charge possibilities the algorithm should look for the peaks. If the spectrum is deconvoluted, this parameter should be 1, as all peaks are represented as charge 1+. Default is 1.
	- **Max. Isotopes**: the number of isotopes the algorithm should look for in each peak. If the spectrum is deconvoluted, this parameter should be 1, as all peaks are represented as monoisotopic. Default is 1.
	- **Deconvolute Spectra**: if this option is checked, the spectra will be deconvoluted before the algorithm looks for the pairs. Default is checked.
	- **Deconvolution Max. Parsimony**: if on, every ion in the experimental spectrum is only allowed to exist within one isotopic envelope (i.e., all isotopic envelopes consist of exclusive ions). Default is on.
	- **Deconvolution PPM**: ppm tolerance for the deconvolution algorithm. Default is 20.
	- **Search for Pairs**: if this option is checked, the algorithm will look for the characteristic pairs from a cross-linking experiment. This is only possible for cleavable cross-linkers. Default is checked.
	- **Search for Reporters**: if this option is checked, the algorithm will look for specific reporter ions generated in the experiment. This option is only possible if the selected cross-linker contains reporter ion. Default is unchecked.
	- **Search for Monolink Pairs**: under implementation.
	- **Crosslinker**: select the crosslinker used in the experiment from a pre-loaded library.
	- **New Crosslinker**: click on this button to build your crosslinker. A new window will appear where you must inform all the properties of your crosslinker, such as the masses of light and heavy fragments, so the shift of the pair can be calculated. You can then add your crosslinker and save your library so it will appear on the Crosslinker options list on the main screen.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/20b8ab34-32aa-4ae6-a70b-12a5f5c233b0" width="650"><br/>

- Results will appear on the main screen, in the form of a boxplot representing the distribution of summed intensities of the highest pair in each spectrum, a bar plot showing the percentage of spectra which contains the doublets, a line plot showing where most pair appear during the chromatography run, and some general information about the crosslinker and the files loaded.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/521cf2f8-6e2c-48ae-9695-f96eb40bfc94" width="650"><br/>

- Double-clicking on one the files shown on the lower right table opens a **Spectra Explorer**, where it’s possible to see exactly which spectra contain the doublets, and which peaks make the pair up.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/7df38b02-f31b-4e67-ab79-e4c233cf7a63" width="650"><br/>

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/c215df3b-fbb6-4a68-853f-88ff2f53f7d2" width="650"><br/>

## Diagnostic Peak Finder

- To run this module, after a spectra file has been loaded, go to the **Analysis** menu.
- There are two options for the Diagnostic Peak Finder:
	- To run on any MS/MS spectra, select **Spectra with min. Xrea** and choose the minimum score for the search (if you want to run this on every scan, select a minimum of zero). Since this is an extensive search, running in this mode may take a while.
	- To try to identify diagnostic peaks only in scans that have been assigned an identification (either PSMs or CSMs) first load an identification file, then select the option **Spectra with ID only**.
- To run the search, click on **Run Diagnostic Peak Finder**.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/a8a23249-7cc5-4a13-b6fe-b3cd05dd3c1e" width="650"><br/>

- Once the search is finished, the results can be seen on the **Diagnostic Peak Finder** tab, in the form of a table detailing the m/z of the peak found, the number of scans it was found in as well as the percentage it represents in the whole run, and the scans’ numbers.

<p align="center"><img src="https://github.com/loukurt/RawVegetable2/assets/63426567/e31b2282-b772-4c0f-9ce9-72f16306b904" width="650"><br/>






