# Step 1: Create and activate the virtual env using conda
create a virtual env using anaconda 

bash 
```
conda create --name culturax python=3.12
```

activate the virtual env


bash

```
conda activate culturax

```


# Step 2: Install the dependencies

run the following command to install the dependencies

bash 

```
pip install -r requirements.txt

```

# Step 3: Add Huggingface Access token

Create your huggingface access token from https://huggingface.co/ and add in config.py in HUGGINGFACE_TOKEN variable

# Step 4 Running the Process for urdu or english dataset

## 4.1: To run the application for Urdu dataset run the following command


bash
```
Python process_ur.py
```

This will create a folder in current directory name as ur_processed_parquet_files which will have the processed parquet files with extracted data as per our requirements and save the files with the same name as the original parquet file name. 

It will also create the list of files in the end which don't have any data we are searching for 

## 4.2: To run the application for Urdu dataset run the following command

Similarly, To run the application for English dataset run the following command

bash
```
Python process_en.py
```

This will create a folder in current directory name as en_processed_parquet_files which will have the processed parquet files with extracted data as per our requirements and save the files with the same name as the original parquet file name. 

It will also create the list of files in the end which don't have any data we are searching for 
