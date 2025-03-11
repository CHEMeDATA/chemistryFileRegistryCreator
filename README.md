# chemistryFileRegistryCreator

Javascript to generate list of chemistry-relevant files from chemistry-data repository

# Installation

```bash
npm install axios
npm install unzipper
```

# Download Zenodo data

To use the Zenodo API, you have to get an [access token](./zenodoToken/README.md). 
Get all records for a given author:
```bash
node src/getRecordForAuthor.js --authorName "Damien Jeannerat" --userName "DamienJeanneratAsUserName"
node src/getRecordForAuthor.js --authorName "Mate Erdelyi" --userName "DamienJeanneratAsUserName"
```

The data are stored in the `./resultsSearch/` folder.

For the record with doi:10.5281/zenodo.3271696:

The compressed archive file is in the `./resultsSearch/Search_1_11_3_2025_14h53m49s/Results/theZenodo_3271696/Content/` folder.

The decompresed files are in the `./resultsSearch/Search_1_11_3_2025_14h53m49s/Results/theZenodo_3271696/Decompressed/` folder.

Metadata are in the `./resultsSearch/Search_1_11_3_2025_14h53m49s/Results/theZenodo_3271696/metadataFile/metadata.json` file.


# Acknowledgements

Some of the methodology and code comes from [Yair](https://github.com/YairRodz), in particular the [ZenodoDownloadAuto repository](https://github.com/YairRodz/ZenodoDownloadAuto) developed during an internship supervised by Damien Jeannerat, Mestrelab Reseach, (Dec. 2023 - March 2024) with funding coming from the [PANACEA consortium](https://www.panacea-nmr.eu/).

