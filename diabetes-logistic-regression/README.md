# Diabetes Prediction with Logistic Regression

This project uses **Logistic Regression** from **scikit-learn** to predict whether a patient has diabetes based on medical diagnostic measurements.

The model is trained and evaluated using the **Pima Indians Diabetes Dataset**.

---

## Dataset

The dataset contains the following features:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

**Target Variable:**

- Outcome
  - 0 = No Diabetes
  - 1 = Diabetes

---

## Technologies Used

- Python
- Pandas
- Scikit-learn

---

## Project Structure

```text
.
├── diabetes.csv
├── diabetes_logistic_regression.py
├── README.md
├── pyproject.toml
```

---

## Installation

Install the required packages:

```bash
uv add pandas scikit-learn
```

or

```bash
pip install pandas scikit-learn
```

---

## Run the Project

Using uv:

```bash
uv run python diabetes_logistic_regression.py
```

or

```bash
python3 diabetes_logistic_regression.py
```

---

## Model Workflow

1. Load the dataset with Pandas.
2. Separate features (`X`) and target (`y`).
3. Split the dataset into training (75%) and testing (25%) sets.
4. Train a Logistic Regression model.
5. Predict diabetes on the test data.
6. Evaluate the model using:
   - Accuracy Score
   - Confusion Matrix

---

## Results

### Accuracy Score

```text
0.7239583333333334
```

### Confusion Matrix

```text
[[95 28]
 [25 44]]
```

---

## Reflection

### Question 1

**How many False Negatives did your model produce?**

The model produced **25 False Negatives**.

### Question 2

**What are the real-world consequences of a False Negative versus a False Positive?**

A **False Negative** means that a patient actually has diabetes, but the model predicts they do not. This can delay diagnosis and treatment, allowing the disease to progress and increasing the risk of serious health complications.

A **False Positive** means that a patient is predicted to have diabetes when they do not actually have it. This may cause unnecessary stress, additional medical tests, and extra healthcare costs, but it is generally less dangerous than a False Negative.

---

## Author

**Atefeh Fahimi Rad**

GitHub:
https://github.com/atefehfahimirad28-droid