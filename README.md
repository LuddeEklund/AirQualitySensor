# AirQualitySensor
Data and Time Series Manipulation with Data Frames

Air sensors collect data about particulate matter in the air (PM10 and PM2.5) and send the data approximately once a minute through a LoRaWAN network to a server. The data is collected on the server on an InfluxDB database. Our sensors are located at the Oodi library in central Helsinki. PM10 describes inhalable particles, with diameters that are generally 10 micrometres and smaller. PM10 also include PM2.5 particles. 
Sometimes there are errors in the data, these errors have to be removed or corrected before further data processing. We have to especially clean away short times spikes before we calculate an hourly PM10 average. 

Our aim is to make a Python program that
1. clean short times spikes from our data, and then
2. calculate the average hourly concentration (µg/ m3) of particulate matter 
In this study, we will use data for dev-id  373773207E330103 and PM10. Our data is collected for a two week period and available as a .csv file. 

Particulate matter, or PM, is a mixture of solids and liquid droplets light enough to float in the air. 
PM10 describes inhalable particles, with diameters that are generally 10 micrometres and smaller. Sources include crushing or grinding operations and dust stirred up by vehicles on roads. 
Fine particles, PM2.5, are 2.5 micrometres in diameter or smaller. Fine particles are produced from all types of combustion, including motor vehicles, power plants, residential wood burning, forest fires, agricultural burning, and some industrial processes
