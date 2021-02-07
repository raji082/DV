# CSE 578 Data Visualization

## VAST 2019 - Micro Challenge 2

### Team Members

* Brahanyaa Somasundaram - 1217364122 - bsomasu1@asu.edu
* Rajasree Chennupati - 1218519276 - rchennu1@asu.edu
* Sai Madhuri Molleti - 1218593116 - smolleti@asu.edu
* Sri Nivethini Vasudevan - 1216804771 - svasud13@asu.edu
* Uma Mageswari Rajendiran - 1217196084 - urajendi@asu.edu
* Subramanya Bhaskara Tarun Lolla - 1216095647 - sbtarun@asu.edu

### Directions to run this code

Our implementation is entirely done using D3.js and this code requires no additional libraries other than D3.js V5. Please ensure to use a local webserver while running this code. Our implementation has been verified using Python's SimpleHTTP Server and also the LiveServer extension in [Visual Studio Code](https://code.visualstudio.com/)

Python's Simple HTTP Server can be initialised as below:

* Syntax: python -m SimpleHTTPServer "PORT NUMBER HERE"

* Example: python -m SimpleHTTPServer 8000

The above command runs the code on the localhost on port 8000.

We have used done some data pre-processing and due to the size constraints of the data, we are uploading this data to [Google Drive](https://drive.google.com/drive/folders/1zv61oq3cSvpWKKsaQRktOp15Rxq4aGxD?usp=sharing). More information about how to obtain the pre-processed data can be found in the Preprocessing section below.

### Data Pre-processing

The data required for this implementation is read from the public directory. The expected data in this directory can be obtained either by downloading the readily available pre-processed data or by manually running the required scripts on the original data.

NOTE: The below files are already present in the Github repository and only the sensors' data needs to be copied to the public folder in the repository.

* choropleth.json
* grids.json
* StHimark.geojson

#### Downloading the Pre-processed Data

The initial files provided for the challenge were too huge and overloaded the browser for every query. Hence, we have pre-processed the given csv files into individual files for each sensor which makes it easy to load only the required data for querying.

Pre-processed Data used for this implementation is available [here](https://drive.google.com/drive/folders/1pDMhHIcOF3EtNCXDt_MXXxYA4czfCg-R?usp=sharing)

This location consists of a zip file - public.zip

Unzip this file to match the below directory structure in the current directory.

* public/sensors
* public/sensors/mobile
* public/sensors/static

#### How to generate the above data?

The initial files provided along with the code to pre-process can be obtained from [here](https://drive.google.com/drive/folders/1o1w9kikcZ79neucXf-DtRq85ggGScrke?usp=sharing) 

The link consists of the preProcess.py file which needs to be present in the same directory as the other .csv and .geojson files provided. The shapefile provided for the challenge has been converted to GeoJSON using the [QGIS3 Tool](https://qgis.org/en/site/) The below directory structure needs to be created before running this file -

* public/sensors
* public/sensors/mobile
* public/sensors/static

After running the script, ensure the data exists in the above mentioned structure. Copy the above public directory to this location while retaining the structure.

### Troubleshooting

We anticipate no technical/functional issues while trying to run this code. However, placing the data files in appropriate locations mentioned above would be key to getting the code to work as expected. The directory structure and the files for this application exist as below -

* css/index.css 
* css/sensors.css
* js/index.js
* js/sensors.js
* public/sensors/static/*.json
* public/sensors/mobile/*.json
* public/StHimark.geojson
* public/choropleth.json
* public/grids.json
* index.html
* sensors.html
* README.md

In addition to this, running this code using a HTTP Server is essential to be able to load the D3.js libraries.