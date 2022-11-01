# Reverse-Image-Search-Scraper
This python notebook can search simultaneously across the 3 following reverse image search engines to scrape image data:

<img src="https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175725.png" width="100">
<img src="https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175806.png" width="100">
<img src="https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175749.png" width="100">

# Deployment

1. Unzip, place the chromedriver in /
2. X virtual framebuffer abbreviated as Xvfb allows you to execute graphical apps without having to use a monitor by connecting some input device. Virtual memory is used to perform graphical operations and it allows the program to run headlessly.

`sudo apt install xvfb`
 
3. git clone https://github.com/Cescollino/Reverse-Image-Search-Scraper.git
4. cd Reverse-Image-Search-Scraper
5. Dependencies
Conda:
The requirements.txt can be used to create a `conda` virtual environment with:
`conda create --name <env> --file requirements.txt`

Virtualenv:
`python3 -m venv scraper`
`source scraper/bin/activate`
`pip install -r requirements.txt`


Once the environment is made, you may open Jupyter Lab and load the notebook, you may use the following command on a terminal:
`jupyter lab`

Open the [Reverse Image Search Scraper.ipynb](/Reverse-Image-Search-Scraper/) in jupyter lab.
Uncomment the first cell and run it once, then comment it again. If there are no errors, you are good to go.

You should see this output:
![image](https://user-images.githubusercontent.com/67806795/199279258-6f63bd16-7e68-4bb5-9110-d1a1c9f0e216.png)

# Defining Paths
Go to the " # Hardcoded File Paths & Run " group of cells

## File Path
You may change the file_path variable to be the absolute path of the image you are trying to upload (.jpg)
ex. (.../Reverse-Image-Search-Scraper/IMAGES/INPUT/1.jpg)

## Result Path
You may change result_path to be the absolute path of the directory you are trying to store your images in.
ex. (.../Reverse-Image-Search-Scraper/IMAGES/OUTPUT)

## Number of Results
You may change the number of results gathered by each engine by changing: "max_count=100" in the last cell of the notebook

## Running
Just press "run all cells".
It may be that there arent any images left for the scraper to download. In that case simply press the square button on the top of the notebook to kill the kernel.

# Output
This program will output image files to the directory with the following nomenclature:

jpg_"Image Number"\_EngineID\_ "Search Engine ID".jpg


![This is an image](https://github.com/Cescollino/Reverse-Image-Search-Scraper/blob/main/Pasted%20image%2020220831175528.png)

# Deduplicating Images
For image nearly similar image deduplication using perceptual hashing, please refer to [imgdupes](https://github.com/knjcode/imgdupes)
