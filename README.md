# SeuratV3Wizard: R Shiny interface for Seurat single-cell analysis library

## Online/Demo:
You can try it online at http://nasqar.abudhabi.nyu.edu/SeuratV3Wizard

## Local Install:

```
devtools::install_github(repo = 'satijalab/seurat', ref = 'release/3.0')
devtools::install_github("nasqar/seuratv3wizard")
```

Optional: For ucsc cellbrowser support, make sure to follow the installation instructions [here](https://cellbrowser.readthedocs.io)

## Run:

```
library(SeuratV3Wizard)
SeuratV3Wizard()
```
This will run on http://0.0.0.0:1234/ by default

## Run using docker:

```
docker run -p 80:80 aymanm/seuratv3wizard
```
This will run on port 80
***

To run on specific ip/port:

```
ip = '127.0.0.1'
portNumber = 5555
SeuratV3Wizard(ip,portNumber)
```
This will run on http://127.0.0.1:5555/

## Screenshots:
![alt text](screenshots/screenshot-input.png "Input Data")

![alt text](screenshots/screenshot-vln.png "Vln Plots")

![alt text](screenshots/screenshot-tsne.png "Cluster Biomarkers")

## Acknowledgements:

1) Rahul Satija, Andrew Butler and Paul Hoffman (2017). Seurat: Tools for Single Cell Genomics. R package version 2.2.1\. [https://CRAN.R-project.org/package=Seurat](https://CRAN.R-project.org/package=Seurat)

2) [Satija Lab](http://satijalab.org/seurat/)
