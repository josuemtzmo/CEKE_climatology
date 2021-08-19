# Climatology, seasonality and trends of oceanic coherent eddies

| Zenodo |
|:------:|
| |

A repository containing material related to the manuscript

> Martínez-Moreno, J., Hogg, A. McC., and England, M. H. Climatology, seasonality and trends of oceanic coherent eddies (To be submitted on April. 2021)

that investigates the seasonal cycle of coherent eddies.

Analysed datasets include the [AVISO+ SSH altimetry](https://www.aviso.altimetry.fr/en/data/products/sea-surface-height-products/global/gridded-sea-level-heights-and-derived-variables.html), identified mesoscale coherent eddies by Chelton & Schlax (2013), and identified mesoscale coherent eddys by TrackEddy (https://github.com/josuemtzmo/trackeddy).

### Python requirements:

Make sure you have the required dependencies installed (`numpy`, `xarray`,`dask`,`cartopy`,`cmocean`, & `jupyterlab`):

```
pip install -r requirements.txt 
```

```
conda install -c conda-forge --file ./requirements.txt
```

Additionally, install [xarrayMannKendall](https://github.com/josuemtzmo/xarrayMannKendall):

```
git clone https://github.com/josuemtzmo/xarrayMannKendall.git
```

and follow the installation instructions in [xarrayMannKendall GitHub Page](https://github.com/josuemtzmo/xarrayMannKendall).

### Contents:

[`manuscript`](https://github.com/josuemtzmo/CEKE_climatology/tree/master/manuscript): folder containing the LaTeX source files and figures for the manuscript

[`datasets`](https://github.com/josuemtzmo/CEKE_climatology/tree/master/datasets): folder in which the NetCDF (`.nc`) output files are expected to be found. Download NetCDF files from <a href="https://doi.org/10.5281/10.5281/zenodo.4646429"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.4646429.svg" alt="zenodo doi"></a>

[`figures`](https://github.com/josuemtzmo/CEKE_climatology/tree/master/figures): folder with jupyter notebooks that produce the main figures of the manuscript.

[`pre-processing`](https://github.com/josuemtzmo/CEKE_climatology/tree/master/pre-processing): folder with scripts and instructions that reproduce `.nc` files in `datasets` from the raw datasets.

### Datasets:
Download the pre-processed datasets from  <a href="https://doi.org/10.5281/zenodo.4646429"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.4646429.svg" alt="zenodo doi"></a>. To facilitate the download of all `*.nc` files, fist install <a href="https://doi.org/10.5281/zenodo.4646429">zenodo_get</a>:

```
pip install zenodo-get
```

Then all the datasets can be downloaded via:

```
cd datasets
zenodo_get 10.5281/zenodo.4646429
```

> **WARNING**: Disk space of ~XX GB is required to download all contents of `datasets` folder.

Now you can reproduce all the analysis and figures of the manuscript; see [`figures`](https://github.com/josuemtzmo/CEKE_climatology/tree/master/figures) folder.

### Authors:
- [Josué Martínez-Moreno](http://josuemtzmo.github.io/) (@josuemtzmo) <[josue.martinezmoreno@anu.edu.au](mailto:josue.martinezmoreno@anu.edu.au)>, 
- [Andy McC. Hogg](http://rses.anu.edu.au/people/academics/prof-andy-hogg) (@AndyHoggANU), 
- [Matthew H. England](http://web.science.unsw.edu.au/~matthew/), 

### Funding:
This study was supported by the ARC Centre of Excellence for Climate Extremes (CLEx) funded by the Australian Research Council, grant CE170100023. In addition:
- J.M.‐M. was supported by the Consejo Nacional de Ciencia y Tecnología (CONACYT), Mexico funding,
- M.H.E. was supported by the Centre for Southern Hemisphere Oceans Research (CSHOR), a joint research centre between  Qingdao National Laboratory for Marine Science and Technology (QNLM), Commonwealth Scientific and Industrial Research Organisation (CSIRO), University of New South Wales (UNSW), and the University of Tasmania (UTAS), and

### Citation:

Cite this repository as:

> XXX

### Software reference:

- David Völgyes, & Rick Lupton. (2020, February 20). Zenodo_get: a downloader for Zenodo records (Version v1.3.0). Zenodo. http://doi.org/10.5281/zenodo.3676567

- Josué Martínez Moreno, & Navid C. Constantinou. (2021, January 23). josuemtzmo/xarrayMannKendall: Mann Kendall significance test implemented in xarray. (Version v.1.0.1). Zenodo. http://doi.org/10.5281/zenodo.4458776
