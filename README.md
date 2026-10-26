# Powerplant_Project
⚡ Predicting power plant energy output (MW) from temperature, vacuum, pressure &amp; humidity using an ANN built in PyTorch. Combined Cycle Power Plant dataset, 9,568 records. machine-learning deep-learning pytorch neural-network regression python pandas scikit-learn data-science energy-prediction 
# ⚡ Power Plant Energy Output Prediction using ANN (PyTorch)

A deep learning regression project that predicts the net hourly electrical energy output (PE) of a Combined Cycle Power Plant from ambient conditions.

## 📊 Dataset
- Combined Cycle Power Plant dataset, 9,568 records, no missing values
- Features:
  - **AT**: Ambient Temperature
  - **V**: Exhaust Vacuum
  - **AP**: Ambient Pressure
  - **RH**: Relative Humidity
- Target: **PE**, Net Hourly Electrical Energy Output (MW)

## 🧠 Model
- Framework: PyTorch
- Architecture: Input (4) → Dense(6, ReLU) → Dense(6, ReLU) → Output(1)
- Loss: MSE | Optimizer: Adam | Epochs: 100 | Batch size: 32
- Train/Test split: 70/30, features scaled with StandardScaler
- Best model saved using validation loss checkpointing (`best_model.pt`)

## 📈 Results
| Metric | Value |
|--------|-------|
| Training MSE | 20% |
| Testing MSE | 19% |
| R² Score | 93% |

## 🛠️ Tech Stack
Python, PyTorch, Pandas, NumPy, Scikit-learn, Matplotlib

## 🚀 How to Run
1. Clone the repo
   `git clone https://github.com/<your-username>/power-plant-energy-prediction-ann.git`
2. Install dependencies
   `pip install pandas numpy scikit-learn torch matplotlib`
3. Open `powerplant.ipynb` in Jupyter and run all cells

## 📁 Files
- `powerplant.ipynb`: full code (preprocessing, training, evaluation)
- `Powerplant_dataset.csv`: dataset

## 🔮 Future Improvements
- Hyperparameter tuning (more layers/neurons, learning rate)
- Compare with Random Forest / XGBoost
- Add feature correlation analysis and a Streamlit app

## 👩‍💻 Author
Nikita Sharma
[LinkedIn](https://linkedin.com/in/nikita-sharma-166626323) | [GitHub](https://github.com/nikushh2006-source)
