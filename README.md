# Data Science Portfolio

## Education

Bachelors of Science (B.S.) Statistics and Data Science – June 2025

## Projects

### Wisconsin Retail and Wholesale Employment Forecasting

Time series forecasting is a core skill in applied statistics and economics. This project was designed to develop expertise in modeling seasonal and trend-based patterns using ARIMA and SARIMA techniques. Forecasting employment trends is critical for informing workforce planning, economic policy, and resource allocation in the public and private sectors. To model employment trends in Wisconsin’s wholesale and retail sectors, I used R to perform time series decomposition, log transformation, and seasonal differencing. I identified model parameters with ACF/PACF plots and selected the best SARIMA model using AICc. Residual diagnostics, including the Ljung-Box and Shapiro-Wilk tests, confirmed model adequacy before generating 12-month forecasts.

**Figure 1** Plot of the original time series. Trend and seasonality is apparent.
![](/assets/img/TSPlot.png)

**Figure 2** Zoomed forecast of original data using chosen model.
![](/assets/img/TSPlot.png)

[View code on Github](https://github.com/uyyrrek/uyyrrek.github.io/blob/main/assets/projects/employee-time-series-forecasting.Rmd)

### Real-Time Twitch Sentiment Analysis

Live chat platforms like Twitch present unique challenges in natural language processing due to informal language, emotes, and rapid message flow. This project serves as a practical application of streaming data pipelines, sentiment analysis, and transformer-based models in a real-time setting. It demonstrates the feasibility of deploying NLP tools for social media monitoring and audience engagement analytics.

**Figure 3** Word cloud caseOH Twitch livestream chat at the time of making the project (March 2025).
![](/assets/img/WordCloud.png)

To analyze audience sentiment during live Twitch streams, I, alongside other members, built a data pipeline that scraped chat messages in real-time using WebSockets. After cleaning and labeling the data, we fine-tuned a RoBERTa transformer model with Hugging Face’s Trainer API in PyTorch. We evaluated both pretrained and custom models to identify sentiment patterns unique to Twitch.

[View code on Colab](https://colab.research.google.com/drive/131jjjYzUcHfstMY-R6EyrSy1ma5Ll0k9?authuser=1)

### Caloric Burn Predictor

This project was inspired by my own personal journey into fitness. As I began exercising more, I became curious about how different physiological and workout factors influence calorie expenditure. I used this curiosity to create a model that helps individuals better tailor their fitness routines to their goals.

Using a public fitness tracking dataset sourced from Kaggle, I applied exploratory data analysis and regression modeling to predict calories burned during exercise. I engineered features from biometric and session-level data—such as heart rate, BMI, and workout type—and trained models to estimate caloric expenditure based on these variables.

[View code on Github](https://github.com/uyyrrek/uyyrrek.github.io/blob/main/assets/projects/calorie-burning-prediction.Rmd)

### Fertility and Infant Mortality Analysis

Using CDC data from 2016–2023, I examined how fertility and infant mortality rates varied across education levels, insurance status, and race. I calculated rates per 1,000 population, reshaped and cleaned the data in R, and visualized stratified trends using `ggplot2`. The analysis revealed public health disparities and correlation patterns across demographic groups.

**Figure 4**
![](\assets\img\FvIMRates.png)

[View code on Github](https://github.com/uyyrrek/uyyrrek.github.io/blob/main/assets/projects/fertility-infant-mortality-analysis.qmd)
