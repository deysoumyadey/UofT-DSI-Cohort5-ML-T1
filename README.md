# UofT-DSI-Cohort5-ML-T1
Team project for UofT-DSI cohort 5 Machine Learning Team 1

Methods and Technologies to Leverage:
Libraries in Python For Machine Learning

Model Examples to Consider:
1. Dense Neural Networks (Fully Connected Networks)
Architecture: Input layer → Multiple dense (fully connected) layers with activation functions (e.g., ReLU) → Output layer (linear activation for regression).
When to Use: Suitable for structured data like numerical or categorical features (e.g., predicting house prices based on features like size and location).

2. Recurrent Neural Networks (RNNs) / Long Short-Term Memory (LSTM) Networks
Architecture: Input (sequence) → LSTM/GRU layers → Dense layers → Output (linear).
When to Use: Best for time-series regression, such as forecasting sales or predicting energy consumption based on historical data.

3. Transformer-Based Models for Regression
Architecture: Input → Transformer encoder layers (multi-head self-attention) → Dense layers → Output (linear).
When to Use: Useful for complex sequential data or when capturing long-range dependencies (e.g., predicting trends in large time-series datasets).

4. Autoencoders for Regression
Architecture: Input → Encoder (dense/conv layers) → Bottleneck → Decoder (optional) → Dense output (linear).
When to Use: Effective for regression with noisy or high-dimensional data, such as denoising sensor data or predicting values from compressed representations.