# Earthquake-Forecasting-Transformer
A Time Series Forecasting project using a custom Transformer architecture to predict earthquake magnitudes based on historical seismic data.


🌍 Earthquake Time Series Forecasting with Transformers
This project implements a Custom Transformer-based Model to forecast earthquake magnitudes. By analyzing sequences of historical seismic activity, the model learns to predict the Richter Magnitude of the next likely event.

📊 Performance & Results
Task: Next-step magnitude prediction.
Input Window: 30 past seismic events.
Model: Multi-head Attention Transformer (PyTorch implementation).
Outcome: The model demonstrates the ability to generalize across different geographical areas (e.g., India, Turkey) and provides magnitude estimates that align closely with historical trends.

📁 Dataset Information
The model is trained on a cleaned seismic dataset.
Features: * Numerical: Latitude, Longitude, Depth, Distance, and various magnitude scales (xm, md, mw, ms, mb).
Categorical: Country, Area, Direction, and detailed time-based features (Year, Month, Day, Hour, Is_Weekend).

Preprocessing: * Date-time feature engineering to extract cyclical patterns.
MinMaxScaler for numerical stability.
Label Encoding for categorical embeddings within the Transformer.

🛠️ Tech Stack
Language: Python
Deep Learning: PyTorch
Data Processing: Pandas, NumPy, Scikit-learn
Visualization: Matplotlib, Seaborn
