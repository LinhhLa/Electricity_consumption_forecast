**Introduction**
This is a course work I created with a team of four. The objective of the assignment was to develop a model to forecast daily logarithmic electricity consumption in Finland for the upcoming day. 
* The model was based on historical data on hourly electricity consumption in Finland and hourly temperature data for three cities: Helsinki, Tampere, and Rovaniemi.
* The forecasts were made in three rounds for 14.3.2024, 16.3.2024, 20.3.2024. Since the objective was to forecast logarithmic daily electricity consumption, the natural logarithm of daily electricity consumption was used in the final forecasts for each round.
* The output of the model was the mean and standard deviation of a forecast value distribution. During model development, AIC and visual investigation of models’ fit were used as criteria for model assessments and selection of the best models.
* The forecasts were assessed based on the log score of the submitted electricity consumption values and the actual consumption for the day of the forecast.

**Preliminary analysis**: The analysis started with exploring the available data on electricity demand in Finland and temperatures provided for Helsinki, Tampere, and Rovaniemi. We plotted the consumption time series data and use scatterplots to see the trend of electricity consumption and temperatures for the three cities.

**Modelling and forecasting**: Our analysis follows the following flow
* Data processing
* Model development
* Conclusions 
