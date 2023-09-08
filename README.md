# Patient-Segmentation-and-Analysis

The goal of this project is to analyze the prescription patterns of the "Target Drug" administered to patients. The objective is to extract dominant prescription patterns from the data using clustering.

## Prerequisites
Before you begin, you will need to have a few tools and libraries installed on your machine:
- Python 3.7 or higher.
- Pandas, Matplotlib, Seaborn, Plotly.
- Scikit-learn.

## Data Inferences

- The dataset contains records for approximately 27,033 unique patients, with prescription data spanning over five and a half years.
- The administration of the "Target Drug" began in February 2017.

## Workflow

### 1. Data Preprocessing

- Addressed basic data inconsistencies.
- Pulled out the positive set relevant to the "Target Drug."
- Sorted the data based on Uid and Date for convenience.

### 2. Feature Engineering

- Engineered a new feature called "Time Interval," representing the interval between subsequent "Target Drug" administrations.
- Handled null values in the "Time Interval" column.

### 3. Clustering Analysis

- Determined the optimal number of clusters using the elbow method.
- Performed k-means clustering and assigned cluster labels to instances.
- Analyzed the percentage distribution of patients in each cluster.

### 4. Visualization and Inferences

- Segregated patients into four clusters for further analysis.
- Visualized prescription patterns for each cluster by plotting the time (months) against the average number of prescriptions.
- Extracted valuable insights from the visualization for each cluster.

## Cluster Analysis

### Cluster 1

- Patients in this cluster took the "Target Drug" for a maximum of 3 months.
- On average, prescriptions were made at least thrice in the first month, twice in the second month, and once in the third month.
- This cluster exhibited a decreasing trend in prescription rates, indicating a need for improved patient engagement.

### Cluster 2

- This cluster demonstrated a consistent and stable pattern.
- Patients in this cluster received prescriptions at regular intervals, with at least one prescription every month from the 9th to the 27th month.
- There was a brief interruption in prescriptions from the 27th to the 32nd month, followed by a resumption of prescriptions every three months.
- This cluster performed well and exhibited a healthy trend.

### Cluster 3

- These patients started taking the "Target Drug" earliest.
- Initially, there were around three prescriptions on average.
- After the first prescription, there was a steep decline in the average number of prescriptions, dropping to less than half of the initial rate.
- Patients in this cluster stopped taking the "Target Drug" within a month, making this cluster the least performing.

### Cluster 4

- Patients in this cluster initially took around one prescription on average for the first six months.
- Afterward, the cluster exhibited a consistent and stable pattern with a slight decline in prescriptions.
- Overall, this cluster performed well, with a relatively shorter duration of around six months.

## Summary

- Clusters 1 and 3, despite having the most patients, performed poorly, with declining trends and short durations of medication.
- Clusters 2 and 4, initially perceived as the worst, performed the best. Cluster 2 exhibited a consistent 18-month pattern, while Cluster 4 showed a stable six-month pattern.
- The project highlights the importance of deeper analysis beyond initial impressions.


## Future Improvements

- Explore other unsupervised techniques for clustering.
- Investigate additional features that could influence prescription patterns.
- Consider patient-specific factors in the analysis.

## Contact
If you have any questions, comments, or suggestions for the project, please feel free to contact me at [nirmal.works@outlook.com]
