@@ -18,16 +18,17 @@ This script assumes that you have already downloaded and unzipped the original S
```
source('download_corpus.R')
```
This will download the corpus and unzip it. Now everything is ready for the analysis.

## how to run the analysis

In your R enviroment, load the script:
In your R enviroment (in the same folder where the data files are), load the script:

```
source('run_analysis.R')
```

This will download the corpus, unzip it and process it. The end result is a file called **'final_tidy_dataset.txt'** in the _output_ folder.
The end result will be a file called `final_tidy_dataset.txt'` in the `output` folder.

```
$ ls output/
@@ -36,9 +37,9 @@ $ ls output/
-rw-rw-r-- 8338031 whole_dataset_with_descriptive_activity_names.csv
```

_final_tidy_dataset.csv_ mirrors the .txt file, in .csv format for your convenience.
_whole_dataset_with_descriptive_activity_names.csv_ is an intermediate file used during the process.
`final_tidy_dataset.csv` mirrors the .txt file in .csv format for your convenience.
`whole_dataset_with_descriptive_activity_names.csv` is an intermediate file used during the analysis.

## final tidy dataset

Each row in the final, clean dataset contains _subject_, _activity_, and measures for all required features (i.e., mean or standard deviation).
Each row in the final, clean dataset contains _subject_, _activity_, and _measures_ for all required features (i.e., mean or standard deviation).