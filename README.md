# ML_Project43-Clustering_TurkeyStudentEvaluation

### Customer Segmentation

This project performs customer segmentation on a dataset containing evaluation scores provided by students from Gazi University in Ankara, Turkey. The goal is to group students into distinct segments based on their responses to 28 Likert-type questions about their course experiences.

### Dataset Information
The dataset contains 5820 evaluation scores from students.

Each record includes the following attributes:

instr: Instructor's identifier (values: 1, 2, 3)

class: Course code (descriptor)

nb.repeat: Number of times the student has taken the course

attendance: Code of the level of attendance

difficulty: Perceived difficulty of the course

Q1-Q28: Likert-type scale responses to 28 course evaluation questions

### Operations Performed

#####Data Loading and Inspection:
The pandas library is used to load the CSV dataset.

Basic data exploration is performed using descriptive statistics and data visualization techniques.

#### Data Preprocessing:
The code checks for missing values and confirms there are none.

##### Exploratory Data Analysis:
The distribution of students across instructors and courses is visualized.

Mean scores for each evaluation question are calculated and visualized.

A correlation matrix is generated to explore relationships between questions.

##### Principal Component Analysis (PCA):
PCA is used to reduce the dimensionality of the data while retaining most of the information.

The explained variance ratio is used to determine how much information is retained.

##### Customer Segmentation:
K-Means clustering is applied to the reduced-dimensionality data using the elbow method to determine the optimal number of clusters.

Students are assigned to clusters based on their responses to the evaluation questions.

The cluster distribution is visualized.

Hierarchical clustering is also performed as an alternative approach.

##### Results

The project successfully segments students into three clusters based on their course evaluation responses. The clusters likely represent different student segments with distinct perceptions of their course experiences.

### Further Exploration

Analyze the characteristics of each cluster to understand the underlying factors that differentiate them.

Investigate the relationship between cluster membership and other student attributes, such as academic performance or demographics.

Explore more advanced clustering algorithms or techniques.

### Code and Libraries Used
```
Python 3
pandas
numpy
seaborn
matplotlib
sklearn
```
