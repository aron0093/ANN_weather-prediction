# ANN_weather-prediction

Historical weather data from Basel is used to predict the amount of *Short wave radiation* on a hourly basis. The data covers 1863 days from 07/2013 to 07/2018. The model is tested on data from 07/2012 to 07/2013.

The input variables used were,

* Hour of day (0-24)
* Temperature (2m above ground)
* Relative Humidity (2m above ground)

This notebook walksthrough the data processing and modelling done for this task. Data can be found [here](https://www.meteoblue.com/en/weather/archive/export/basel_switzerland_2661604?daterange=2013-07-19+to+2018-07-18&params=&params%5B%5D=11%3B2+m+above+gnd&params%5B%5D=52%3B2+m+above+gnd&params%5B%5D=71%3Bsfc&params%5B%5D=204%3Bsfc&utc_offset=2&aggregation=hourly&temperatureunit=CELSIUS&windspeedunit=KILOMETER_PER_HOUR).

For building the model I use the keras scikit-learn API. While this API constrains us to single input models, it does feel familiar to anyone already acustomed to this interface and provides all the expected functionality.

I am using the tensorflow backend for keras (this is also the default setting) and have not used GPU accelaration for this model. This code will work regardless if anyone does run it on any other backend.

**Note** keras version 2.1.4 was used

