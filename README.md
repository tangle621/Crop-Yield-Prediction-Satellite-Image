# Crop Yield Prediction with Satellite Images

**Table of Contents**
- [Objective](#objective)
- [How to run the pipline](how-to-run-the-pipeline)
- [Data Acquisition](#data-acquisition)
- [Derived Insights]()
- [Crop-Classification]()


## Objective
This project's objective is to minigate the supply chain risks in food and agricultural sectors by predicting crop yields in France. <br>
The pipeline is to be integraged into [Agrisight®](https://agrisight.emerton-data.com/?page_id=320&lang=en) by [Emerton Data®](https://www.emerton-data.com/)

## Descroption of Pipeline
Although there are 2,200 satellites flying nowadays, usage of satellite image (remote sensing data) is limited due to the scientific and technical difficulties to acquired and process them properly. This pipleline will allow user to automatically acquire and process Sentinel-2 data, and calculate vegetation indices by running one single script.<br>
With this, your team will be capable to start analysing the data right away and run any models you wish.<br>
Desired time range, area, and kind of vegetation indices is easily configurable thanks to the structure.<br><br>

As the code is highly confidential for our clients, if you would like to have a demo of our packages, please contact me.

## How to run the pipeline
This pipeline automatically acquire and process satellite image, 
Create log file
```python
mkdr logs
```
Initialize the vertual environment
```python
pipenv install
pipenv shell
```

Run code
```python
python run.py 
```
