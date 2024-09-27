## Training an ML Model on Historical Minute Bar Data

This example showcases the power of Amazon SageMaker in training an XGBoost model (or any time series model, such as GluonTS) using historical minute bar data. With just a few lines of Python code, you can leverage SageMaker's managed Jupyter notebook instance and distributed training capabilities to efficiently train your model on large datasets.

Check out more: [XGBoost Model training](./algodev-sagemaker.ipynb) 

## Backtesting the ML Model

After training your ML model, it's crucial to evaluate its performance through backtesting. This process not only validates the model's effectiveness but also helps derive a robust trading strategy. SageMaker streamlines the backtesting process by allowing you to load historical minute bar data and run your backtesting code seamlessly within the managed Jupyter notebook environment.

Check out more: [Model backtesting](./backtest-sagemaker.ipynb) 


## Training time series model

Forecasting volume accurately is crucial for achieving a reliable Volume Weighted Average Price (VWAP). This example showcases how to load historical minute bar data and train a [DeepAR](https://docs.aws.amazon.com/sagemaker/latest/dg/deepar.html) model on SageMaker to forecast volume effectively.

The process begins by loading the historical minute bar data, which typically includes timestamps, volume, and other relevant features. The data is then preprocessed and transformed into a format suitable for training the DeepAR model. Once trained, the DeepAR model can be used to forecast future volume, enabling more accurate VWAP calculations and informed trading decisions. 

Check out more: [DeepAR time series model training](./algodev-sagemaker-deepar.ipynb)