# Compare_Schedulling_Algorithms-OS-

This project compares several CPU scheduling algorithms using Python and Jupyter Notebook.

## Overview

The notebook simulates and analyzes four classic scheduling algorithms:
- **FCFS (First-Come, First-Served)**
- **SJF (Shortest Job First, Non-preemptive)**
- **SRTF (Shortest Remaining Time First, Preemptive)**
- **RR (Round Robin)**

It generates random process arrival and burst times, runs each scheduling algorithm, and prints detailed results. A final table compares average turnaround and waiting times for each algorithm, and results are visualized using matplotlib.

## Features

- Generates a set of random processes with arrival and burst times (default: 25 processes).
- Implements classic scheduling algorithms in an object-oriented approach.
- Prints a table of process statistics after each scheduling run.
- Compares algorithms in a summary table.
- Plots results for visual comparison.

## Usage

1. Open `sheduling.ipynb` in Jupyter Notebook or Google Colab.
2. Run the notebook cells.
3. When prompted, enter a seed number for reproducible random data.
4. Enter a time quantum for Round Robin when prompted.
5. Review printed tables and plots.

## Requirements

- Python 3
- `matplotlib`
- `numpy`

## Example Output

The notebook prints tables like:

```
PID | Arrival | Burst | Completion | Waiting | Turnaround
----+---------+-------+------------+---------+-----------
  1 |       1 |     2 |          8 |       5 |          7
  ...
Average Waiting Time: 68.24
Average Turnaround Time: 74.84
```

Comparison table:

```
Algorithm | Avg TAT | Avg WT 
----------+---------+--------
FCFS      |   74.84 |  68.24
SJF       |   59.28 |  52.68
SRTF      |   59.16 |  52.56
RR        |  104.64 |  98.04
```

## License

MIT
