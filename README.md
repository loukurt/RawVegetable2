# RawVegetable 2.0
A quality control software with specialized modules for XLMS experiments. RawVegetable 1.0 can be found at http://patternlabforproteomics.org/rawvegetable/

# Equipment
## Hardware
A computer with a minimum of 16 GB RAM and 4 computing cores is recommended. However, the software can take advantage of superior configurations.
## Software
- Windows 10 (64 bits) or later.
- The .NET Core 6 or later, which can be downloaded at https://dotnet.microsoft.com/en-us/download/dotnet/6.0
- The RawVegetable software, available for download at https://github.com/diogobor/RawVegetable2/releases

# Tutorial
## Loading Spectra Files
-	Spectra data can be loaded from files in the *.raw, *.mzML, *.ms1 or *.mgf formats, by either dropping them on the main screen or by clicking at **File** and then **Load Files**. Multiple files can be loaded at the same time. (Note: for *.ms1 files, RawVegetable will attempt to find the respective *.ms2 file necessary for some modules, if it cannot be found, the features will be disabled. The same will happen for *.mgf if it only contains MS1 spectra)

![Picture1](https://github.com/loukurt/RawVegetable2/assets/63426567/91b8c8b5-6210-48f2-ba66-b69d8c0ba99e)

![Picture2](https://github.com/loukurt/RawVegetable2/assets/63426567/8b0012c6-c8a8-4ac3-8fb5-f9d19b59a25c)

## Navigating Open Files

- The user has full control of which files should be displayed in the screen and used for specific modules by opening the **Open Files** menu once the files have loaded and (un)checking the specific files/plots.

![Picture3](https://github.com/loukurt/RawVegetable2/assets/63426567/3184857c-4564-4d5f-bc89-cf52d84474c7)

- It’s also possible to change the colours used for each file by right-clicking on the name of the file.

![Picture4](https://github.com/loukurt/RawVegetable2/assets/63426567/5a63c103-5c42-46f3-a944-0ce99c8315b9)

