# Online Course Engagement Prediction

## Overview

This project predicts whether an online course will be **completed** or remain **pending** based on learners’ engagement patterns such as time spent, quizzes taken, videos watched and device usage.
It uses **Logistic Regression**, **Support Vector Machines (SVM)**, and **Random Forest Classifier** to classify course completion outcomes.

---

## Dataset Description

The dataset `predictOnlineCourseEngagementDataset.csv` contains the following features:

| Feature                   | Description                                               |
| ------------------------- | --------------------------------------------------------- |
| **UserID**                | Unique ID for each learner (removed for model training)   |
| **CourseCategory**        | Course type: Health, Arts, Science, Programming, Business |
| **TimeSpentOnCourse**     | Time spent on the course (hours)                          |
| **NumberOfVideosWatched** | Count of videos watched                                   |
| **NumberOfQuizzesTaken**  | Count of quizzes attempted                                |
| **QuizScores**            | Average quiz score                                        |
| **CompletionRate**        | Percentage of course completed                            |
| **DeviceType**            | Device used (Desktop/Mobile)                              |
| **CourseCompletion**      | Target label: Completed or Pending                        |

---

## Steps & Methods

1. **Data Preprocessing**

   * Removal of unnecessary columns (`UserID`)
   * Encoding categorical variables (`CourseCategory`, `DeviceType`, `CourseCompletion`)
   * Handling missing values
   * Descriptive statistics and data type inspection

2. **Exploratory Data Analysis (EDA)**

   * **Histograms** for feature distribution
   * **Boxplots** to detect outliers
   * Summary statistics

3. **Model Building**

   * **Logistic Regression**
   * **Support Vector Machine (SVM)**
   * **Random Forest Classifier**
   * Accuracy and classification reports for each model

4. **User Input Prediction**

   * Custom input prompts to predict if a course will be completed or not

5. **Statistical Testing**

   * **Z-test**: To compare sample completion rates against population mean
   * **Chi-Square test**: To analyze relationships between categorical features

---

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | \~79%    |
| SVM                 | \~83%    |
| Random Forest       | \~96%    |

---

## Technologies Used

* Python
* Pandas
* Matplotlib & Seaborn
* Scikit-learn
* NumPy & SciPy

---

## How to Run

1. Clone the repository

   ```bash
   git clone https://github.com/Syeda-Mahjabin-Proma/Online-Course-Engagement-Prediction.git
   ```
2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Python script

   ```bash
   python main.py
   ```

---

## Future Improvements

* Add more features like **geographic location** or **learning pace**
* Hyperparameter tuning for better accuracy
* Deploy as a **web application** for real-time predictions
