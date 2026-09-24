# Operating System Scheduling Algorithms

A Python project exploring and visualizing classic **CPU scheduling algorithms** through simulated processes and jobs.

The project implements both **non-preemptive and preemptive scheduling strategies**, calculates scheduling metrics, and generates Gantt-style visualizations to make the behavior of each algorithm easier to understand.

## Algorithms

### Process Dispatcher

- **FCFS** — First Come, First Served
- **SPN** — Shortest Process Next
- **HRRN** — Highest Response Ratio Next
- **RR** — Round Robin
- **SRTF** — Shortest Remaining Time First

### Job Scheduler

- **FIFO / FCFS**
- **SJF** — Shortest Job First
- **Random** scheduling

## Features

- Simulates processes with different arrival and CPU burst times
- Handles idle periods between processes
- Visualizes scheduling using Gantt-style charts
- Calculates:
  - Average Waiting Time
  - Average Turnaround Time
  - Algorithm Execution Time
- Includes functionality for comparing scheduling algorithms based on waiting time and execution time

## Requirements

Install the required Python libraries with:

    pip install pandas numpy matplotlib seaborn

## Usage

The project can be run directly from Python. Example datasets and test cases are included in the source files.

For example:

    calculate(FCFS, df1)

Multiple algorithms can also be compared:

    the_best([FCFS, SPN, HRRN, RR, SRTF], df2)

Algorithms requiring a time quantum, such as **Round Robin** and **SRTF**, prompt for the time slice when executed.

## Project Structure

    .
    ├── dispatcher.py
    ├── job_scheduler.py
    └── README.md

## Purpose

This project was built as a hands-on exploration of **operating system scheduling concepts**, combining algorithmic implementation with visual simulation and performance analysis.
