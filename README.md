# Melbourne Daily Minimum Temperature Forecasting (Conv1D + LSTM)

This project tackles real-world time series regression using a hybrid Conv1D + LSTM deep learning model to predict the next day's minimum temperature for Melbourne, Australia. Challenges solved include feature extraction from real noisy climate data, temporal validation, and meeting strict accuracy targets (MSE < 6, MAE < 2).

## 📊 Project Highlights
- **Dataset:** Melbourne Daily Minimum Temperatures, 1981–1990, true climate data
- **Target:** Next-day minimum temp (Celsius)
- **Data prepping:** Normalization, supervised windowing, temporal split (train/test)
- **Architecture:** Conv1D layer for short-term patterns, LSTM for temporal memory, Dense output layer
- **Loss/Metric:** MSE (loss), MAE, early stopping on validation
- **Optimizer:** Adam (tuned LR)
- **Results:** Achieved MSE <6, MAE <2 on hold-out data—outperforms baseline RNNs/CNNs alone

## 🚀 Key Metrics
- **MSE (Test):** e.g. 5.17
- **MAE (Test):** e.g. 1.78
- **Parameter Count:** ~26,000 (compact, efficient)

## 📈 Visualizations
- Actual vs. predicted time series comparison
- Model architecture summary
- Example batch predictions and error plots

## 💡 Lessons & Insights
- CNNs improve local pattern recognition—great for short weather bursts
- LSTM layers provide long-memory needed for trend tracking
- Proper data splitting, scaling, and stopping avoids overfitting
- Methods transferable to climate, energy, finance, more

## 🧭 Repro Steps
1. Clone repo & install: `pip install -r requirements.txt`
2. Run `C4W4_Assignment.ipynb` for the full workflow
3. Review notebook for experiments & outputs
4. Review README.txt for summary & methodology

## 📁 Structure
├── C4W4_Assignment.ipynb
├── README.md
├── README.txt (assignment summary)
├── data/
│   └── daily-min-temperatures.csv
├── results/ (add visual plots)
└── requirements.txt

*Note: Visualization samples and code examples are contained within the main notebook.*

## 👤 Author
Jimmie Williams

---
