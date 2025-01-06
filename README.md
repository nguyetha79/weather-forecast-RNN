# Weather Forecasting using RNN

In the context of the course 'Foundations of Computational Intelligence,' I have carried out a related project that demonstrates how to use Recurrent Neural Networks (RNNs) with Long Short-Term Memory (LSTM) units for weather forecasting to explore the impact of context size. The notebook `zeitreihenprognose_wettervorhersage.ipynb` includes the following key steps:

1. **Setup and Data Preparation**:
   - Installation of required libraries including TensorFlow.
   - Loading and normalizing the Jena Climate dataset, which consists of various weather attributes recorded every 10 minutes.

2. **Data Visualization**:
   - Visualizing raw data to understand the patterns and distributions of different weather features.

3. **Data Preprocessing**:
   - Down-sampling the data to reduce the number of data points.
   - Normalizing the selected features to standardize the input values.

4. **Dataset Creation**:
   - Splitting the data into training and validation sets.
   - Creating time series datasets using the `timeseries_dataset_from_array` method from Keras.

5. **Model Building**:
   - Defining the LSTM model architecture with input, LSTM, and dense layers.
   - Compiling the model with the Adam optimizer and Mean Squared Error loss function.

6. **Training the Model**:
   - Training the model with the training and validation datasets.
   - Using callbacks for early stopping and saving the best model checkpoints.

7. **Evaluation**:
   - Evaluating the model performance using Mean Absolute Error (MAE).
