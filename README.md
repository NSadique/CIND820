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
<p>The dataset is available on <a href="hhttps://www150.statcan.gc.ca/t1/tbl1/en/cv.action?pid=3210012501">Statistics Canada</a>.</p>
<p>A basic cleaned version of the dataset is available on this repository looking at cattle counts for slaughet and mass of cattle per year since 1920.</p>
<p>As of this moment, the variables looked are the Total Cattle Count (Cattle and Calves) per year for the ARIMA and LSTM models.</p>

<h2>Technique and Tools</h2>
<p>This project will be done using Python and libraries such as Pandas, Numpy, keras, sklearn, and others for visualization.</p>
<p>Currently these 2 approaches are being used for modeling, a third one will be selected (most likely NBeats)</p>
<ol>
    <li>ARIMA Model</li>
    <li>LSTM Model</li>
    <li>NBeats Model (looking into)</li>
</ol>

<h2>Initial Preparation</h2>
<p>Plotting the data to see if there is any trends in the data and whether seasonal patterns are present.</p>
![Cattle Count per Year](https://raw.githubusercontent.com/NSadique/CIND820/main/Images/Initial%20Plot.png)<br>
