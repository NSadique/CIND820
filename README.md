<h1>Predicting Cattle Growth or Decline in Canada</h1>

Author: Naveed Sadique <br>
CIND820: Big Data Analytics Project<br>
Project Supervisor: Dr. Sedef Akinli Kocak<br> 

<h2>Purpose</h2>
<p>This project looks at Canada dataset for Cattle Counts accross Canada.<br>
The main goal of this project is to create a predictive model of cattle to determine the future growth or decline of cattle.<br>
The current trend looks to be a downward trend in the cattle count. However, looking into the counts and weight, we can see total amount of beef availabe. <br>
If the total amount of beef is increasing or decreasing, then we can answer questions whether beef consumption in Canada has decreased or if the beef supply is being handled internationally from external studies.<br>
<br>
Currently, the focus has been creating a model to predict cattle counts.</p>

<h2>Repository Contents</h2>
<p>This repository contains the original dataset, a cleaned version of the dataset, and intiial models for cattle counts done via ARIMA and LSTM</p>

<h2>Data</h2>
<p>The dataset is available on <a href="https://www150.statcan.gc.ca/t1/tbl1/en/cv.action?pid=3210012501">Statistics Canada</a>.</p>
<p>A basic cleaned version of the dataset is available on this repository looking at cattle counts for slaughet and mass of cattle per year since 1920.</p>
<p>As of this moment, the variables looked are the Total Cattle Count (Cattle and Calves) per year for the ARIMA and LSTM models.</p>

<h2>Evaluation</h2>
<p>Model Evaluation metrics will be:</p>
<ol>
    <li>RMSE</li>
    <li>MAD</li>
    <li>MAE</li>
</ol>

<h2>Technique and Tools</h2>
<p>This project will be done using Python and libraries such as Pandas, Numpy, keras, sklearn, and others for visualization.</p>
<p>The following approaches are going to be used to create time-series models for forecasting:</p>
<ol>
    <li>ARIMA Model</li>
    <li>LSTM Model</li>
    <li>NeuralProphet</li>
</ol>

<h2>Requirements</h2>

* Python

<p>As well as the following libraries:</p>

* Pandas
* Numpy
* Statsmodels
* matplotlib
* math
* Keras
* sklearn
* NeuralProphet

<h2>Methodology</h2>

| Step | Description |
|------|-------------|
|Problem Definition|To identify cattle population trends and to determine whether the population is trending down or up|
|Data Preparation|Review gaps in data to make sure no missing values for all segments, remove data not being used for modeling|
|Data Preprocessing & Exploration|Look at impacts of normalization and differencing. Decided to look at creating models without normalizing, normalizing, and differencing|
|Model Building & Testing|Generate models for ARIMA, LSTM, and NeuralProphet to work with the available data|
|Analysis|Split the dataset into training and testing data. Review results via required metrics and look at actuals and predicted|
|Results Validation|Interpret the results for all preprocessed data and compare metrics to the appropriate scale to review performance|
|Interpretation|Communicate results and conclusions for models and presented results|

<h2>Results</h2>

|Model| Dataset|RMSE|MAD|MAPE| SmoothL1Loss |
|-------|------|------|-----|------|--------------|
|ARIMA  |Cattle|281.335|199.437|0.059||
|ARIMA  |Calve|16.128|13.264|0.045||
|ARIMA|Cattle(norm)|0.079|0.056|0.455||
|ARIMA|Calve(norm)|0.013|0.011|0.029|
|LSTM|Cattle(diff)|91.936|57.878|0.900||
|LSTM|Calve(diff)|24.033|14.307|1.067||
|LSTM|Cattle(undiff)|287.871|218.804|0.083||
|LSTM|Calve(undiff)|107.869|73.235|0.090||
|NeuralProphet|Cattle|405.350|333.610||0.010|
|NeuralProphet|Calve|189.350|180.800||0.020|
|NeuralProphet|Cattle(norm)|0.120|0.100||0.010|
|NeuralProphet|(Calve(norm)|0.140|0.130||0.010|

<h2>Conclusions</h2>
<p>The cattle counts in Canada for meat production have begun a downward trend from the established high from the 1970s. The models have predicted a continue decline in cattle counts which does fall in line with changes in societal and economical values. Red meat consumption has been proven to be vastly unhealthier compared to other meats and many alternative preoteins are targeting the red meat food markets. </p>

<p>Additional studies have shown that the consumption of red meats produced by cattle have decreased and the acceptance of alternative options are growing in favour. In general in economics as the demand for a product diminishes, the supply will have to adjust to maintain equillibrium, which can explain the begining downward trend. Growing economic costs of red meat compared to alternative have also impacted purchasing habits and thus red meat might not be as profitable to produce compared to the past (further research required).</p>

<p>The models generated should be applicable to general cattle population samples, however additional features and additional datapoints will allow for more accurate forecasting models. Further research should involve looking at the types of cattle being produced, as well the number of cattle put to slaughter. Having more factors available will also allow the model to have more verstatility to be applicable to other livestock markets.</p>

