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

## Example Output

| Metric   | Count | Mean    | Std Dev | Min   | 25%    | 50%    | 75%    | Max      |
|----------|-------|---------|---------|-------|--------|--------|--------|----------|
| CPU      | 1440  | 20.48   | 8.12    | 4.29  | 16.45  | 19.96  | 23.45  | 99.83    |
| RAM      | 1440  | 40.44   | 10.94   | 8.07  | 33.39  | 40.28  | 47.09  | 99.53    |
| Disk     | 1440  | 103713  | 45568   | 38584 | 87073  | 100322 | 113650 | 681443   |
| Network  | 1440  | 208337  | 100257  | 42163 | 168428 | 201591 | 234745 | 1481568  |

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
