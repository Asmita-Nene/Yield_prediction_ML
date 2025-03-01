# Yield_prediction_ML
<h3>Overview</h3>
This project uses mini batch SGD linear regression to predict the yield of a field based on rainfall recieved. The project involves data preprocessing, data visualization, model training and model evaluation using a seperate testing dataset.<br/>
<h3>Project Description</h3>
This project creates a linear regression model that uses rainfall_mm as a feature to predict the yield_in_ton_per_hectare of a field</br>
The dataset of the project was taken from the website - https://www.kaggle.com <br/>
Link for dataset - https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield<br/>
<br/>
The dataset was first checked for any missing values and it had no missing values.<br/>
This dataset was then split into a training dataset and a testing dataset for proper result analysis. This training dataset was used to create a correlation matrix and a pairplot. By analysis of both the correlation matrix and pairplot, it was observed that the label "Yield_tons_per_hectare" had the strongest correlation with the feature "Rainfall_mm".<br/>
Python Keras library was used for creation and training of the  linear regression model. The results were analysed using the plot of loss curve and the plot of dataset and the most fit line of the model.<br/>

<h3>Technology used </h3>
<ul>
  <li>Python Jupyter Notebook</li>
  <li>Python Pandas library - for dataset handling.</li>
  <li>Python Keras Library - for training and implementation of ML model.</li>
  <li>Python Plotly Library - for data visualization.</li>
  <li>Python Seaborn Library - for data visualization.</li>
</ul><br/>

<h3>Dataset Description</h3>
The dataset contains agricultural data for 1,000,000 samples. The dataset contains the following factors - <br>
<ul>
<li>Region</li>
<li>Soil_Type</li>
<li>Crop </li>
<li>Rainfall_mm</li>
<li>Temperature_Celsius</li>
<li>Fertilizer_Used</li>
<li>Irrigation_Used</li>
<li>Weather_Condition</li>
<li>Days_to_Harvest</li>
<li>Yield_tons_per_hectare</li>
</ul>
Out of all these factors, it was observed that the rainfall_mm had the strongest correlation with the yield in ton label. Hence, the model was trained with only one feature that was the "Rainfall_mm" feature to predict the value of the label "Yield_tons_per_hectare".<br/>

<h3>Results</h3>
After training the linear regression model, the following result was obtained - <br/>
RMSE = 1.096 <br/>
This value of error can be further reduced by fine tuning of the hyperparameters.<br/>
