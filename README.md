# Reverse-Image-Search-Scraper
This python notebook can search across the 3 following reverse image search engines to scrape image data:

![[Pasted image 20220831175725.png]]
![[Pasted image 20220831175749.png]]
![[Pasted image 20220831175806.png]]

# Installing Environment
The requirements.txt can be used to create a `conda` virtual environment with

`conda create --name <env> --file requirements.txt`

Once the environment is made, you may open Jupyter Lab and load the notebook.

# Defining Paths
Go to the " # Hardcoded File Paths & Run " group of cells

## File Path
You may change the file_path variable to be the absolute path of the image you are trying to upload (.jpg)

## Result Path
You may change result_path to be the absolute path of the directory you are trying to store your images in.

# Output
This program will output image files to the directory with the following nomenclature:

jpg_"Image Number"\_EngineID\_ "Search Engine ID".jpg

![[Pasted image 20220831175528.png]]
