# CPM and PERT Analysis Tool

This repository provides a Python implementation of the Critical Path Method (CPM) and Program Evaluation and Review Technique (PERT). It is designed to analyze project schedules, identify critical tasks, and estimate the probability of meeting project deadlines. The project uses a real-world dataset for demonstration purposes.

## Features

- **Critical Path Method (CPM):**
  - Calculates the earliest start (ES) and finish (EF) times for each task.
  - Determines the latest start (LS) and finish (LF) times to identify slack time.
  - Identifies the critical path of the project, which dictates the minimum project duration.

- **Program Evaluation and Review Technique (PERT):**
  - Incorporates optimistic, pessimistic, and most likely durations to estimate expected task durations and variances.
  - Calculates the probability of completing the project within a given timeframe using a normal distribution.

- **Graphical Visualization:**
  - Generates a clear and organized project network diagram for better task dependency understanding.

## Dataset

The tool uses a dataset containing project tasks and their attributes. The key columns include:

- `Ref`: Task reference ID
- `Status`: Task status (e.g., Open, Closed)
- `Description`: Description of the task
- `Task Group`: Logical grouping of tasks
- `Duration`: Task duration (calculated or predefined)
- `Optimistic`, `Most_Likely`, `Pessimistic`: Durations for PERT calculations

## Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```

2. Install required Python libraries:
   ```bash
   pip install pandas matplotlib networkx scipy
   ```

## Usage

1. Place your dataset in CSV format at the appropriate file path.
2. Update the `file_path` variable in the script to point to your dataset.
3. Run the Python script to:
   - Perform CPM analysis.
   - Perform PERT analysis.
   - Visualize the project network diagram.

### Running the Code
```bash
python cpm_pert_analysis.py
```

## Outputs

- **Critical Path Identification:** Outputs the critical tasks of the project.
- **Project Duration Estimates:** Provides expected project duration and variance.
- **Probability of Meeting Deadlines:** Calculates the likelihood of completing the project within a specified timeframe.
- **Visualization:** Displays a graphical representation of the project network.

## Example Results

1. **Critical Path:**
   ```
   Critical Path: T1 -> T2 -> T3
   ```

2. **Expected Project Duration:**
   ```
   Expected Project Duration: 15 days
   ```

3. **Probability of Meeting Deadline:**
   ```
   Probability of completing the project within 20 days: 95.87%
   ```

4. **Graphical Output:**
   A clear project network diagram with nodes representing tasks and edges representing dependencies.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributions

Contributions are welcome! Feel free to submit issues or pull requests to improve this tool.

## Contact

For questions or feedback, please reach out to [ImBlackline](https://github.com/imblackline).

