# Anomaly Detection in System Resource Usage

This project provides a Jupyter Notebook for monitoring and analyzing system resource usage-including CPU, RAM, disk, and network activity-with a focus on anomaly detection using statistical methods.

---

## Features

- Collects system metrics (CPU, RAM, disk, network) using Python libraries.
- Provides statistical summaries (count, mean, std, min, max, quartiles) for each resource.
- Calculates z-scores for CPU and RAM usage to identify anomalies.
- Suitable for time-series analysis and visualization of system health.

---

## Technologies Used

- `pandas` for data manipulation and analysis
- `psutil` for accessing system resource metrics
- `matplotlib` for plotting and visualization

---

**Sample Data with Z-Scores**

| Timestamp           | CPU   | RAM   | Disk      | Network   | Z-Score CPU | Z-Score RAM |
|---------------------|-------|-------|-----------|-----------|-------------|-------------|
| 2025-05-09 00:00:00 | 22.95 | 26.08 | 122393.01 | 135523.15 | 0.30        | -1.31       |
| 2025-05-09 00:01:00 | 14.79 | 22.15 | 90181.34  | 214086.74 | -0.70       | -1.67       |
| 2025-05-09 00:02:00 | 24.64 | 44.67 | 114729.46 | 220857.67 | 0.51        | 0.39        |

---

## Usage

1. Clone this repository.
2. Install dependencies:
```bash
pip install pandas psutil matplotlib
```
3. Open the notebook (`anomaly.ipynb`) in Jupyter.
4. Run the cells to monitor and analyze your system's resource usage.

---

## Applications

- Real-time system monitoring
- Anomaly detection for performance troubleshooting
- Data collection for capacity planning

---

## License

This project is open source and available under the MIT License.

---

## Acknowledgments

- Built using open-source Python libraries.
- Inspired by the need for simple, effective anomaly detection in system resource monitoring.

---

*For questions or contributions, please open an issue or submit a pull request.*

