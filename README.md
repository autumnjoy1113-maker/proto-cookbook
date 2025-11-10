# Autumn's Prototype Cookbook Using ERA5 and Last Millenium Reanalysis Data to Visulaize Precipitation In Alabama

<img src="thumbnails/thumbnail.png" alt="thumbnail" width="300"/>

[![nightly-build](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/cookbook-template/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/cookbook-template/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/475509405.svg)](https://zenodo.org/badge/latestdoi/475509405)


This Project Pythia Cookbook covers precipitation variability in Alabama using both modern reanalysis data (ERA5) and paloeclimate reconstructions (NOAA's LAst Millennium Reanalysis, LMR). Through these Jupyter notebooks we analyze rainfall patterns, and visualize long-term trends.

## Motivation

Understanding Alabama’s hydroclimate through both instrument and proxy records helps reveal the natural range of precipitation variability and contextualize recent changes in the climate system.

By completing this cookbook, you’ll gain skills in:

- Loading and exploring NetCDF and Zarr datasets using xarray and pandas

- Subsetting regional climate data using latitude/longitude bounds

- Visualizing precipitation trends, anomalies, and century-scale distributions

- Interpreting reanalysis and paleoclimate data for regional applications

## Authors

[Autumn Johnson](https://github.com/first-author1)


## Structure

This cookbook is organized into two main notebooks:


### ERA5 Modern Precipitation Analysis

This notebook:

Loads ERA5 monthly mean reanalysis data (Zarr format)

Selects the Alabama region based on latitude/longitude bounds

Visualizes precipitation time series and seasonal climatologies

Includes markdown commentary and conclusions about 20th–21st century rainfall trends

### LMR Paleoclimate Precipitation Analysis

This notebook:

Loads Last Millennium Reanalysis (LMR) NetCDF data from NOAA Paleoclimatology

Extracts Alabama’s region and computes ensemble mean precipitation

Aggregates values by century and visualizes boxplots and mean trends

Compares variability across major paleoclimate intervals (e.g., Medieval Climate Anomaly, Little Ice Age)

Concludes with markdown summaries linking proxy-derived variability to modern reanalysis trends

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.


### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter).

Note, not all Cookbook chapters are executable. If you do not see
the rocket ship icon, such as on this page, you are not viewing an
executable book chapter.


### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

(Replace "cookbook-example" with the title of your cookbooks)

1. Clone the `https://github.com/ProjectPythia/cookbook-example` repository:

   ```bash
    git clone https://github.com/ProjectPythia/cookbook-example.git
   ```

1. Move into the `cookbook-example` directory
   ```bash
   cd cookbook-example
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate cookbook-example
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
