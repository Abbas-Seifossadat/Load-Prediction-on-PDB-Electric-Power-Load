# Daily Peak Load Forecasting with LSTM-Attention Model  

This repository contains the implementation of a machine learning pipeline for forecasting daily peak energy demand using a Long Short-Term Memory (LSTM) model with an Attention mechanism. The project demonstrates an end-to-end methodology, from preprocessing time series data to optimizing model hyperparameters and evaluating the results, with an emphasis on high accuracy and interpretability.  

---

## Project Overview  

Accurate load forecasting is crucial for efficient energy management and infrastructure planning. This project leverages:  
- **Advanced Time Series Processing**: Creating sequence data from hourly demand to predict daily peak loads effectively.  
- **LSTM with Attention**: Utilizing the attention mechanism to enhance the model’s ability to focus on relevant temporal patterns.  
- **Hyperparameter Optimization**: Employing **Optuna**, a state-of-the-art optimization framework, to fine-tune hyperparameters for optimal model performance.  

---

## Methodology  

1. **Data Preprocessing**  
   - Extracted peak daily demand from hourly energy usage data.  
   - Sequence creation based on Autocorrelation Function (ACF) to identify the optimal sequence length.  
   - Applied scaling and splitting techniques to prepare training and validation datasets.  

2. **Model Architecture**  
   - An LSTM-based model with an Attention mechanism to improve focus on critical time dependencies.  
   - Dense layers with dropout regularization for robust learning.  

3. **Hyperparameter Optimization**  
   - Utilized Optuna to search for the best configuration of LSTM units, dense layers, dropout rates, and learning rates.  

4. **Model Evaluation**  
   - Assessed performance using Mean Absolute Error (MAE) and visualized predictions against actual demand.  

---

## Results  

- Achieved excellent performance with an MAE of **0.00435** on validation data.  
- Early stopping at **29 epochs** ensured efficient training.  
- Visualized predictions demonstrate strong alignment with actual demand trends.  

---

## How to Run  

1. Clone this repository:  
   ```bash  
   git clone https://github.com/yourusername/peak-load-forecasting.git  
   cd peak-load-forecasting  
   ```  

2. Install the required dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Run the Jupyter Notebook:  
   ```bash  
   jupyter notebook Load_Prediction.ipynb  
   ```  

---

## Dependencies  

- Python 3.8+  
- TensorFlow 2.x  
- Optuna  
- Numpy, Pandas, Matplotlib, Plotly  

---

## Key Features  

- **Attention Mechanism**: Improves LSTM’s interpretability and prediction accuracy.  
- **Optuna Hyperparameter Tuning**: Automates hyperparameter search for efficient model optimization.  
- **ACF-Based Sequence Selection**: Ensures optimal sequence length for time series modeling.  

---

## Insights  

This project highlights the potential of advanced machine learning techniques to address real-world challenges in energy management. The LSTM-Attention model delivers high accuracy and robustness, making it suitable for deployment in dynamic energy forecasting applications.  

---

## Future Work  

- Incorporating external features such as weather forecasts or socio-economic data to improve model performance.  
- Exploring other deep learning architectures like Transformer-based models for comparative analysis.  

---

## Contact  

For any queries or contributions, feel free to reach out:  
- **Abbas Seifossadat**: [abbas.seifossadat@gmail.com](abbas.seifossadat@gmail.com)
- **Alireza Feizbakhsh**: [Feizbakhsh22@gmail.com](Feizbakhsh22@gmail.com)  
- LinkedIn: [Abbas Seifossadat](www.linkedin.com/in/abbas-seifossadat-563756106)  
- LinkedIn: [Alireza Feizbakhsh](https://www.linkedin.com/in/alireza-feizbakhsh-98706772/)  