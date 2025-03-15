# EUMDAC for Data Store

**EUMDAC_for_data_store** is a collection of Python-based code designed to demonstrate the capability of, and provide training on, the use of the EUMETSAT's data services and provided Python interface EUMDAC.

[TOC]

## How to use this course material

These lessons will first walk you through how to discover, browse, search and download products in the EUMETSAT Data Store, using the EUMDAC Python library. At the end of this part of the tutorial, you should be able to interface with the EUMETSAT Data Store catalogue using a programmatic framework.

In the second part of the course, we will focus on how customise products with the EUMETSAT Data Tailor, using the EUMDAC Python library. At the end of this part of the tutorial, you should be able to configuring your own chains and start customisations of products from Data Store through the Data Tailor.

## Authors
* [**Ben Loveday**](mailto://ops@eumetsat.int) - *Initial work* - [EUMETSAT](http://www.eumetsat.int)
* [**Niklas Jordan**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
* [**Valters Zeizis**](mailto://ops@eumetsat.int) - [EUMETSAT](http://www.eumetsat.int)
 
## Getting Started
  
The course is based on [Jupyter notebooks](https://jupyter.org/), which allow a high-level of interactive learning, as code, text description and visualisation is combined in one place. If you have not worked with 
`Jupyter Notebooks` before, you can look at the module [Introduction to Python and Project Jupyter](0_Intro_to_Python_and_Jupyter.ipynb) to get a short introduction to Jupyter notebooks and their benefits.

This repository is focussed on using **Data Store** and the **Data Tailor** (web-service and as a local instance) and their APIs, mainly with the Python library provided by the **EUMETSAT Data Access Client (EUMDAC)**. If you need more background on how EUMDAC works and which capabilities it has, you can check out the [EUMDAC documentation](https://user.eumetsat.int/resources/user-guides/eumetsat-data-access-client-eumdac-guide).

You will need an access token to use certain parts of the APIs. For the token generation you'll need your personal API keys, you find here [https://api.eumetsat.int/api-key](https://api.eumetsat.int/api-key) module.

### Prerequisites
 
You will require Jupyter notebook to run this code. We recommend that you install the latest Anaconda Python distribution for your operating system (https://www.anaconda.com/). Anaconda Python distributions include Jupyter Notebook.

Addationally, this course is mainly based on the Python library provided by the EUMETSAT Data Access Client (EUMDAC). You have to install the EUMDAC package first in the same environment as you want to run the notebooks. Find the different ways to install the package in the EUMDAC user guide: https://user.eumetsat.int/resources/user-guides/eumetsat-data-access-client-eumdac-guide#ID-Installing-EUMDAC

### Running Jupyter notebooks

To to run Jupyter Notebooks, open an Anaconda prompt and make sure you have activated the correct environment. Again, navigate to the root directory. Once you are in the correct directory, run Jupyter using `jupyter notebook` or `jupyter-notebook`(depending on your operating system).

This should open Jupyter Notebooks in a browser window. On occasion, Jupyter may not be able to open a window and will give you a URL to past in your browser. Please do so, if required.

## Materials

The course follows a modular approach and offers the following sections, each divided into several modules:

### 0. Introduction (Optional)
 1. [**Intro to Python and Project Jupyter**](0_Intro_to_Python_and_Jupyter.ipynb)<br />This module will introduce you into the Jupyter environemt, how to install it and use the notebooks in this repository.

### 1. Data Store

 1. [**Discovering collections**](1_1_Discovering_collections.ipynb)<br />This module will show you how to discover EUMETSAT Data Store collections with the EUMDAC Python client and how to get the collection ID.
 2. [**Searching and filtering products**](1_2_Searching_and_filtering_products.ipynb)<br />This module will show you how to search for and discover products in a collection and filter them by both area and time.
 3. [**Downloading products**](1_3_Downloading_products.ipynb)<br />This module will show you how to download whole products or just a single file from a product in various ways.
 4. [**Sentinel-3 Data Store access**](1_4_Sentinel3_data_access.ipynb)<br />This module will show you how to bring the search, filtering and downloading processes described in the previous modules, with a focus on Sentinel-3 data.
 5. [**MTG FCI Data Store access**](1_5_MTG_FCI_data_access.ipynb)<br/>This module will show you how to search, filter and download products or individual components of products from the MTG FCI Level-1C collection.
 6. [**Accessing MTG LI products**](1_6_MTG_LI_data_access.ipynb)<br/>This module will show you how to search, filter and download MTG LI products as well as how to aggregate multiple chunks in a full-day product or into a single CSV file.

### 2. Data Tailor Web Service

 1. [**Using the Data Tailor with EUMDAC**](2_1_Customising_products.ipynb)<br/>This module will show you how to select a product from the Data Store and pass it to Data Tailor to remotely customise it before downloading.
 2. [**Cleaning the Data Tailor workspace**](2_2_Cleaning_the_Data_Tailor_workspace.ipynb)<br/>This module will show you how to retrieve all your customisation jobs and clear one or more of them from your workspace.

### 3. Data Tailor Standalone

 1. [**Using the Data Tailor Standalone with EUMDAC**](3_Data_Tailor_standalone.ipynb)<br/>This module will show you how to download a product from the Data Store and pass it to your local Data Tailor instace for further customisation.

### 4. EUMDAC Cookbook

 1.  [**EUMDAC Cookbook**](4_EUMDAC-Cookbook.ipynb)<br />A curated collection of practical code examples designed to help users navigate the complexities of accessing and processing data from EUMETSAT's Data Access Services using the EUMDAC Python Library.