# PID Controller Optimization using Machine Learning

🚀 A project that uses a neural network to predict optimal PID (Kp, Ki, Kd) parameters based on step response characteristics.

## 📦 Dataset

- Synthetically generated using MATLAB Simulink simulation
- Each row contains:
  - Inputs: Rise Time, Overshoot, Settling Time, Steady-State Error
  - Targets: Kp, Ki, Kd (scaled)

> Dataset generated and exported using `Simulation.slx`  
> Format: [CSV] + [Preprocessed NPZ]

---

## 🛠 Tools Used

| Tool         | Purpose                              |
|--------------|---------------------------------------|
| Python       | Data processing & model training      |
| TensorFlow   | Neural network architecture           |
| MATLAB       | Generate control response data        |
| Power BI     | Visualize predicted results           |

---

## 🧠 ML Model Summary

- Inputs: 4 features (RiseTime, Overshoot, SettlingTime, SS_Error)
- Outputs: 3 targets (Kp, Ki, Kd)
- Loss: `Mean Squared Error`
- Activation: ReLU + Linear Output
- Optimizer: Adam with learning rate tuning

---

## 📊 Dashboard (Power BI)

- Visual comparison of `Actual vs Predicted` PID values
- Interactive filters (e.g. error range)
- KPI cards summarizing prediction errors
- ![Performance Dashboard](images/Performance.jfif)

---

## 📁 Folder Structure

- `/data/`: Cleaned data and scalers
- `/notebooks/`: Model training & analysis
- `/simulation/`: Simulink files for generating data
- `/dashboard/`: Power BI reports and outputs
- `/images/`: Screenshots for documentation

---

## 🧪 Future Work

- Integrate model with real-time control simulation
- Try Reinforcement Learning for adaptive tuning

---

## 📌 Credits

- Dataset generated via custom simulation

