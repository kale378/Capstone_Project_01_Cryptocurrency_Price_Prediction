# Capstone_Project_01_Cryptocurrency_Price_Prediction

Title: Capstone Project - Cryptocurrency Price Pridiction Analysis

Introduction: our project focused on predicting cryptocurrency prices using a method called time series analysis. Imagine if we could use past price patterns to guess 
how prices might change in the future. Just like how weather forecasts use past weather patterns to predict upcoming weather, we're using past cryptocurrency price patterns 
to predict their future values. This could be really helpful for people who invest in cryptocurrencies or just want to understand where their values might be headed. 
We'll be exploring different ways to make these predictions and hoping to learn more about how these digital currencies behave over time.

Problem Statement: The problem we're tackling is that it's really hard to predict how cryptocurrency prices will change. This makes it tricky for people who want to invest 
in cryptocurrencies or make smart decisions about them. Cryptocurrency prices can go up and down a lot, and if we can't predict these changes, it's easy to lose money.
So, our project's problem is to find ways to use past price information to guess where these prices might go in the future. This could help people make smarter choices
when dealing with cryptocurrencies and avoid potential losses.

Data Collection: To train and evaluate the Cryptocurrency Price pridiction analysis model, a substantial amount of hotel review data is required. The project likely involved 
accessing existing publicly available datasets containing Past Records of cryptocurrencies. The data would include different variable i.e. 'High', 'Low', 'Open', 'Close', 
'Date' and 'Price'.

Exploratory Data Analysis(EDA): However, I can outline the general steps involved in performing Exploratory Data Analysis (EDA) for Cryptocurrency price prediction analysis 
project. The EDA process typically involves the following:

   1.  Data Loading: The Jupyter Notebook would start by loading the dataset containing bit coin data and corresponding Price. The data may be in various formats
       such as CSV, Excel, or JSON.

   2.  Data Inspection: The notebook would display basic information about the dataset, such as the number of rows and columns, data types,
       and the presence of missing values.

   3.  Drop Duplicates: In this particular dataset too many duplicated rows are present, I removed that futhermore there are many duplicate dates are also present I also
       deal with that. And futher prediction are done on data that remain after deleting the duplicate records.

   4.  Type_Casting: Here I covert the date variable from string to date-time format.

   5.  Set_Index: In time series we have to work on only two variables so that the date is set as index and sort it according to date.

   6.  Decompostion: Decomposition in time series involves breaking down a series into its key components: trend, seasonality, and noise. The trend represents the
       overall direction of the data, whether it's going up or down over time. Seasonality captures regular patterns or cycles that repeat at specific intervals.


Remember that the specific EDA steps may vary depending on the dataset and the goals of the project. The EDA part serves as a crucial foundation for understanding the 
data and making informed decisions for subsequent stages in the "Cryptocurrency price orediction Analysis" Capstone Project.

Data Preprocessing: extensive preprocessing is necessary before being used for model training. The preprocessing steps for this project might include convertin Categorical
Variable into date-time,Normalisation. Here in this dataset there is a problem for normalization because here some data is already normalised(last) and some records are not
so here very carefully I handle this problem.

Train-Test-Split: Here based on the past 50 records I predict the future values.

Model Building: In this project I Used different algorithms of Deep Learning which Include:

   1. Long short term memory(LSTM):  using a powerful type of artificial intelligence called LSTM to predict future values in time series data  like cryptocurrency prices.
      LSTM can remember important patterns over long periods, making it great for understanding and forecasting trends in things that change over time,
      like stock prices or weather conditions. This helps us make more accurate predictions about where the data is headed.

   2. Simple RNN: employing Simple Recurrent Neural Networks (RNNs) to predict future values in time series data like cryptocurrency prices. Simple RNNs have the ability
      to consider past information and use it to make predictions about what might happen next. This is really handy for understanding and forecasting patterns in data that
      evolves over time, such as stock prices or sales figures. Our aim is to harness the power of Simple RNNs to make informed predictions about where the data could
      be heading.

   3. Gated Recurrent Unit(GRU): using Gated Recurrent Units (GRUs) to predict future values in time series data, such as cryptocurrency prices. GRUs are a type of
      neural network that's great at capturing patterns in sequences. They're especially useful for understanding and predicting trends in data that changes over time,
      like stock prices or temperature fluctuations. By leveraging the capabilities of GRUs, we aim to enhance our ability to make accurate predictions about the future
      direction of the data.

  Conclusion: Here all three algorithms give approximately equal accuracy. but simple RNN has minimum 'Root mean Squared' value. so we can finalize the Model with Simple 
              RNN algorithm.

