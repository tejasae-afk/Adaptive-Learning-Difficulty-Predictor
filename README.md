# Adaptive-Learning-Difficulty-Predictor
Students often struggle with one-size-fits-all education systems that ignore individual differences. This project proposes a machine learning–based adaptive learning system that predicts students’ learning difficulty levels and recommends personalized learning strategies.

In many traditional education systems, students are taught in the same way, even though people learn very differently. Because of this, students who struggle are often noticed only after their performance drops a lot. The goal of this project is to deal with that problem by building a machine learning–based adaptive learning system that predicts a student’s learning difficulty and suggests learning strategies that fit their needs.

The project uses a real Student Performance dataset from Kaggle, which includes academic, demographic, and behavioral data for students taking Portuguese and Mathematics courses. After combining both datasets, the final data contains 1,044 students with 33 features, such as exam scores (G1, G2, G3), study time, absences, and past failures.

To make prediction easier, an average academic score is calculated using G1, G2, and G3. Based on this score, students are grouped into Low, Medium, or High learning difficulty levels. In addition to the original features, some behavioral features are created, like learning pace, attendance ratio, and academic consistency. These features help describe how students learn, not just how they perform on exams.

Two models are trained and compared. Logistic Regression is used as a baseline because it is simple and easy to interpret. Random Forest is used as the main model since it can handle more complex patterns in the data. The Random Forest model performs better overall and gives balanced results across all difficulty levels.

The project also looks at fairness by checking how predictions are distributed across genders. The results do not show any major imbalance, which suggests the model does not introduce clear gender bias.

An early warning model is also built using only early indicators like study time, absences, failures, and the first exam score. This allows the system to identify students who may need support before final exam results are available.

Overall, this project shows how machine learning can be used to support early intervention and more personalized learning, instead of treating every student the same.
