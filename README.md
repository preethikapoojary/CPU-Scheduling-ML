# ML-Based CPU Scheduling Strategy Prediction

## Project Overview
This project uses Machine Learning to predict the most suitable CPU scheduling algorithm based on process workload characteristics.

It combines traditional CPU scheduling algorithms with a Machine Learning ensemble model using Random Forest and XGBoost with Soft Voting.

## Objectives
- Generate diverse CPU process workloads.
- Implement and compare CPU scheduling algorithms.
- Analyze scheduling performance using different metrics.
- Train Machine Learning models to recommend suitable scheduling strategies.
- Build an interactive CPU scheduling prediction demo.

## CPU Scheduling Algorithms
1. **FCFS (First Come First Serve)** – Executes processes in arrival order.
2. **SJF (Shortest Job First)** – Selects the available process with the shortest burst time.
3. **Priority Scheduling** – Executes processes based on priority.
4. **Round Robin** – Allocates CPU time using a fixed time quantum of 4.

## Machine Learning Models
The project compares:
- Random Forest
- Decision Tree
- XGBoost
- Neural Network

**Final Ensemble Model:**
- Random Forest
- XGBoost
- Combination technique: Soft Voting

## Dataset
- Generated workloads: 5,000
- Total process records: 47,580
- Features used: 17
- Training samples: 4,000
- Testing samples: 1,000

## Performance Metrics
The scheduling algorithms are compared using:
- Waiting Time
- Turnaround Time
- Response Time
- Throughput
- Context Switches
- CPU Utilization

## Reported Model Results

| Model | Accuracy |
|---|---:|
| Random Forest | 90.5% |
| Decision Tree | 86.1% |
| XGBoost | 87.9% |
| Neural Network | 88.0% |
| RF + XGBoost Ensemble | 88.7% |

*Note: The dataset has an imbalanced class distribution, so accuracy should be considered alongside balanced accuracy and Macro F1.*

## Technologies Used
- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Joblib

## Project Workflow
1. Generate diverse CPU workloads.
2. Implement FCFS, SJF, Priority and Round Robin.
3. Calculate scheduling performance metrics.
4. Generate and validate the ML dataset.
5. Train and compare Machine Learning models.
6. Build the Random Forest + XGBoost ensemble.
7. Predict the most suitable scheduling strategy.
8. Compare all four scheduling algorithms for a user-entered workload.

## How to Run
1. Open the notebook in Google Colab.
2. Run the notebook cells in sequence.
3. Generate the workload dataset.
4. Train the Machine Learning models.
5. Enter process details in the prediction demo.
6. View the recommended scheduling strategy and performance comparison.

## Conclusion
This project demonstrates how Machine Learning can be integrated with Operating System CPU scheduling concepts to recommend scheduling strategies based on workload characteristics.

## Author
Preethika Poojary
