# Predicting Heart Disease Using Machine Learning

This notebook looks into using various Python-based machine learning and data science libraries in an attempt to build a machine-learning model capable of predicting whether someone has heart disease based on their medical information.

Built with:
<br>
<br>
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
<br>
<br>
![Jupyter Notebook](https://img.shields.io/badge/jupyter-fff.svg?style=for-the-badge&logo=jupyter&logoColor=orange)
<br>
<br>
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
<br>
<br>
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) 
<br>
<br>
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) 
<br>
<br>
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
<br>
<br>


We are going to take the following approach:
1. Problem Definition
2. Data
3. Evaluation
4. Features
5. Modeling
6. Experimentation

## 1. Problem Definition
> Given clinical parameters about a patient, can we predict whether they have heart disease?

## 2. Data
- The original data came from the Cleveland data from the UCI Machine Learning Repository. [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+Disease)
- There is also a version of it available on Kaggle. [Kaggle Heart Disease Dataset](https://www.kaggle.com/ronitf/heart-disease-uci)

## 3. Evaluation
> If we can reach 95% accuracy at predicting whether a patient has heart disease during the proof of concept.

## 4. Features
**Heart Disease Data Dictionary**

The following are the features we'll use to predict our target variable (heart disease or no heart disease).

1. **age** - age in years
2. **sex** - (1 = male; 0 = female)
3. **cp** - chest pain type
   - 0: Typical angina: chest pain related decrease blood supply to the heart
   - 1: Atypical angina: chest pain not related to heart
   - 2: Non-anginal pain: typically esophageal spasms (non heart related)
   - 3: Asymptomatic: chest pain not showing signs of disease
4. **trestbps** - resting blood pressure (in mm Hg on admission to the hospital). Anything above 130-140 is typically cause for concern
5. **chol** - serum cholesterol in mg/dl. Serum = LDL + HDL + .2 * triglycerides. Above 200 is cause for concern
6. **fbs** - (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false). '>126' mg/dL signals diabetes
7. **restecg** - resting electrocardiograph results
   - 0: Nothing to note
   - 1: ST-T Wave abnormality (can range from mild symptoms to severe problems, signals non-normal heart beat)
   - 2: Possible or definite left ventricular hypertrophy (enlarged heart's main pumping chamber)
8. **thalach** - maximum heart rate achieved
9. **exang** - exercise induced angina (1 = yes; 0 = no)
10. **oldpeak** - ST depression induced by exercise relative to rest (looks at stress of heart during exercise; unhealthy heart will stress more)
11. **slope** - the slope of the peak exercise ST segment
    - 0: Upsloping: better heart rate with exercise (uncommon)
    - 1: Flatsloping: minimal change (typical healthy heart)
    - 2: Downsloping: signs of unhealthy heart
12. **ca** - number of major vessels (0-3) colored by fluoroscopy (colored vessels means the doctor can see the blood passing through; the more blood movement the better, no clots)
13. **thal** - thallium stress result
    - 1, 3: normal
    - 6: fixed defect: used to be defect but ok now
    - 7: reversible defect: no proper blood movement when exercising
14. **target** - have disease or not (1 = yes, 0 = no)

## 5. Installation

### 5.1 Prerequisites

- [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) (Anaconda or Miniconda distribution)
- [Git](https://git-scm.com/)

### 5.2 Installing Dependencies
#### Option 1: Using Conda

1. **Clone the repository:**

    ```bash
    git clone https://github.com/AdrianTomin/heart-disease-prediction.git
    cd heart-disease-prediction
    ```

2. **Create and activate the Conda environment:**

    ```bash
    conda env create -f environment.yml
    conda activate heart-disease-classification
    ```

#### Option 2: Using pip

1. **Clone the repository:**

    ```bash
    git clone https://github.com/AdrianTomin/heart-disease-prediction.git
    cd heart-disease-prediction
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

Choose one of these options to set up the environment, depending on your preference.
`

### 5.3 Setting Up the Environment

1. **Install Jupyter Notebook or JupyterLab:**

    ```bash
    conda install -c conda-forge notebook
    # or for JupyterLab
    conda install -c conda-forge jupyterlab
    ```

2. **Start Jupyter Notebook or JupyterLab:**

    ```bash
    jupyter notebook
    # or for JupyterLab
    jupyter lab
    ```

## 6. Running the Project Locally

1. **Navigate to the project directory:**

    ```bash
    cd heart-disease-prediction
    ```

2. **Start the Jupyter Notebook server:**

    ```bash
    jupyter notebook
    ```

3. **Open the notebook:**

    In the Jupyter Notebook interface, open the `heart_disease_prediction.ipynb` notebook.

4. **Run the notebook cells:**

    Execute the cells in the notebook to train the model and make predictions. Ensure you have downloaded the dataset and placed it in the appropriate directory as mentioned in the notebook.

---

This README provides a comprehensive guide for setting up the environment, installing dependencies, and running the notebook.


## Badges
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

## Authors
- [@AdrianTomin](https://www.github.com/AdrianTomin)
