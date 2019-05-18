# IEOR242-SFCrimePrediction

GitHub Repository for IEOR242 Final Project

Datasets: 
* [San Francisco Crime Data, 2003-2018](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry)
* [Eviction Notices, 1997-2019](https://data.sfgov.org/Housing-and-Buildings/Eviction-Notices/5cei-gny5)
* [RedFin Housing Market Data, 2012-2019](https://www.redfin.com/blog/data-center?fbclid=IwAR3sW7Mb0S4Ausofnk2BEnNAlx4RlMpKqBM1sW7wS6GkKwdTTzho6lNxKq8)
* [Daily sunrise and sunset timings](https://sunrise-sunset.org/) - accessed by API

The code is separated into two folders, [preprocessing](preprocessing) and [modeling](modeling). 

In the preprocessing folder, 'datasetsCleaned.ipnyb' is the main notebook to run. The complementary notebook 'sunrisesunset-webcrawling.ipnyb' is the script to obtain the sunrise and sunset timings from the Open Source API.

For the modelling files, they are to be in the following sequence: 'modeling.ipnyb' and 'modeling II.ipnyb'. The first notebook uses the daily dataset, and the second notebook extends upon the daily dataset by adding a binary feature of daytime/nighttime based on the sunrise and sunset timings, and a feature for time of day. The LSTM models should be run in this sequence:
a) modelling III - a (time series).ipynb
b) modeling - LSTM part a.ipynb
c) modeling - LSTM part b.ipynb
