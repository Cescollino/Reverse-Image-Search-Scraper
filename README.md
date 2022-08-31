# Reverse-Image-Search-Scraper
This python notebook can search simultaneously across the 3 following reverse image search engines to scrape image data:

<img src="https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175725.png" width="100">
<img src="https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175806.png" width="100">
<img src="https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175749.png" width="100">

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


![This is an image](https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175528.png)
