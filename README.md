# sampling_assignment
This solution aims to:

• Convert an imbalanced dataset into a balanced dataset

• Apply five different sampling techniques

• Train five different machine learning models

• Compare model performance using accuracy

• Identify which sampling technique performs best for each model

⚙️ Methodology

The complete workflow consists of six major stages:

1️⃣ Data Loading & Preprocessing

The dataset is loaded using pandas

Features (X) and target (y) are separated

No data leakage is allowed between training and test sets

2️⃣ Balancing the Dataset

To eliminate class imbalance:

Random Oversampling is applied

Minority class samples are duplicated until both classes have equal representation

✅ Outcome:
A balanced dataset where both classes have equal sample counts.

3️⃣ Sampling Techniques Applied

Five sampling techniques were selected from the provided list:

Sampling ID	Technique	Description
Sampling1	Simple Random Sampling	Randomly selects records
Sampling2	Systematic Sampling	Selects every k-th record
Sampling3	Stratified Sampling	Preserves class proportions
Sampling4	Cluster Sampling	Samples data from selected clusters
Sampling5	Bootstrap Sampling	Sampling with replacement

Each sampling technique generates a new sample from the balanced dataset.

4️⃣ Machine Learning Models Used

Five machine learning models were trained on each sampled dataset:

Model ID	Algorithm
M1	Logistic Regression
M2	Decision Tree
M3	Random Forest
M4	Support Vector Machine
M5	K-Nearest Neighbors

All models were trained using:

70% training data

30% testing data

Feature scaling using StandardScaler where required

5️⃣ Performance Metric

Accuracy (%) was used as the evaluation metric

Best Sampling Technique per Model:

M1: Sampling5 (93.67%)

M2: Sampling5 (100.0%)

M3: Sampling1 (100.0%)

M4: Sampling2 (99.13%)

M5: Sampling5 (98.25%)

Accuracy is suitable here because the dataset was balanced before training.
