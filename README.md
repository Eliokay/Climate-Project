# Climate-Project
## Project Description
Using over 80  years of daily sea surface temperature (SST) data from the South Atlantic ocean basin, the purpose of this project is to examine for evidence of long-term trends such as warming ocean temperatures and more frequent or intense storms. 

## Data Description
ERA5 is produced by the European Center for Medium-Range Weather Forecasting (ECMWF), widely regarded as the best forecasting center in the world. The SST data from the South Atlantic ocean was queried from the ERA5 Reanalysis Product. This dataset combines historical observations with physics based computer models of the earth systems to produce consistent global datasets. 

## Data Analysis
To assist with this analysis, I posed the question: are there discernible trends in the dataset, and if so, can they be projected into the future? I began by loading the dataset into my Colab notebook, where I inspected the rows and columns. Given that this was a time series dataset, I decided to conduct a spectral analysis, focusing on the power spectral density of the SST with respect to its daily frequency measurements.
Upon generating the spectral graph, I identified significant peaks and trends, noting a distinct annual cycle. To further isolate this yearly trend, I applied a Butterworth low-pass filter, which effectively smoothed the data by attenuating high-frequency noise while preserving the low-frequency components associated with the annual cycle.
To forecast this trend, I used the Prophet Model Regressor. Additionally, I conducted a comparative analysis by creating a second model using the SST signal from the entire dataset. This allowed me to evaluate how predictions using the SST differed from those based solely on the filtered SST signal.

## Requirements
This project was carried out using Google Colaboratory 

## Author
This project was created and carried out by [Eloho Okoloko](https://www.linkedin.com/in/elohookoloko/). 

## License
[MIT]([https://github.com/Eliokay/Climate-Project/blob/main/LICENSE]) © Eloho Okoloko
