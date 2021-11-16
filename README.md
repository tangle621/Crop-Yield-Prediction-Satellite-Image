# Crop Yield Prediction with Satellite Image
<p align="center">
<img src="./images/satellite.png" alt="satellite" width="300">
</p>

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->

**Table of Contents**
- [Conterxt & Objective](#objective)
- [About our pipeline](#about-our-pipeline)
  - [Description](#description-of-pipeline)
  - [Data acquisition mechanism](#data-acquisition-mechanism)
  - [How to run the pipline](#how-to-run-the-pipeline)
- [Enabled work results](enabled-work-examples)
  - [Derive insights](#derive-insights)
  - [Crop-classification](#crop-classification)
<!-- markdown-toc end -->


# Objective
Harvest are naturally seasonal, meaning that once harvest season has passed, deliveries are made throughout the year, diminishing a fixed amount of initial
stock. This means that there is a specific need to plan out the way stocks will be chipped off over time, in order not to initially over-sell (not as trivial as it sounds accounting for multiple qualities and geographic locations), optimize the use of logistics networks (Optimal Transport problem) and finally make smart pricing decisions.

This project's objective is to mitigate the logistics and profitability risks for food and agricultural sectors by predicting crop yields in France. <br>
The pipeline is to be integraged into [Agrisight®](https://agrisight.emerton-data.com/?page_id=320&lang=en) by [Emerton Data®](https://www.emerton-data.com/)

# About our pipeline

## Description
Although there are 2,200 satellites flying nowadays, usage of satellite image (remote sensing data) is limited due to the scientific and technical difficulties to acquired and process them properly. This pipleline will allow user to automatically acquire and process Sentinel-2 data, and calculate vegetation indices by running one single script.<br>
With this, your team will be capable to start analysing the data right away and run any models you wish.<br>
Desired time range, area, and kind of vegetation indices is easily configurable thanks to the structure.<br><br>
As the code is highly confidential, if you would like to have a demo of beta version, please contact us.

## Utilized data
- Sentinel 2 <br>
Sentinel 2 is an earth observation mission from ESA Copernicus Program. <br>
It provides high resolution satellite images (10m - 60m) over land and coastal waters, with a large spectrum and a high frequency (~5 - 15 days) <br>

- French national registry <br>
A national register of cereal fields is publicly available. <br>
It provides: <br>
The GPS coordinates of fields, defining the exact polygon <br>
The type of crop grown in each field by year <br>

- Crop yield data <br>
Crop yiled data was acquired from a local farmer in France. <br>


## Data acquisition mechanism

<p align="center">
<img src="./images/data_acquisition.png" alt="data_acquisition">
</p>

## How to run
Pipeline is runnable in any environment with a virtual environment.<br>
First, create log file
```python
mkdr logs
```
Initialize the virtual environment
```python
pipenv install
pipenv shell
```

Run code
```python
python run.py 
```

# Enabled works examples
## Derive insights
<p align="center">
<img src="./images/vi_evolution_map.png">
</p>
<br><br>

<p align="center">
<img src="./images/vi_evolution_lineplot.png">
</p>
<br><br>

<p align="center">
<img src="./images/vi_evolution_heatmap.png">
</p>
<br><br>

<p align="center">
<img src="./images/lr.png" width="800">
</p>
<br><br>

## Crop classification
<p align="center">
<img src="./images/classification_result.png">
</p>
<br><br>

## Crop yield prediction
<p align="center">
<img src="./images/time_series.png">
</p>
