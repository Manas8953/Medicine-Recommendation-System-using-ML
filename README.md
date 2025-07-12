# 🩺 Disease Prediction and Recommendation System

This project leverages machine learning to predict diseases based on user-input symptoms and provides actionable recommendations including precautions, medications, workout, and dietary suggestions.

## 🚀 Project Highlights

- Achieved **100% accuracy** on test data using a **Support Vector Classifier (SVC)** trained on a **multi-class dataset with 133 features** and 4920 records.
- Designed a custom symptom-to-disease prediction pipeline by encoding user symptoms into a binary input vector based on a comprehensive symptom dictionary.
- Integrated multiple datasets (`precautions`, `workout`, `diet`, `medications`, and `disease descriptions`) to provide a complete, explainable, and human-centric recommendation system.
- Stored and reused trained model via `pickle` for real-time predictions.
- Ensured modular architecture with helper functions for mapping disease → actionable health suggestions.

## 💡 Tech Stack

- Python (NumPy, Pandas, Scikit-learn)
- Machine Learning: Support Vector Classifier (SVC)
- Data Processing: Label Encoding, Binary Vectorization
- Deployment-ready format using `pickle`

## 📌 Usage

1. Input symptoms as comma-separated values.
2. Model predicts the most probable disease.
3. System provides:
   - Description of the disease
   - 4 key precautions
   - Recommended medications
   - Suggested workouts
   - Diet chart

## 🗂️ Datasets Used

- `symptoms_df.csv`
- `precautions_df.csv`
- `medications.csv`
- `description.csv`
- `workout_df.csv`
- `diets.csv`

## ✅ Example

```plaintext
Input: yellow_crust_ooze, red_sore_around_nose, small_dents_in_nails, inflammatory_nails, blister

Predicted Disease: Impetigo

Precautions:
1. Soak affected area in warm water
2. Use antibiotics
3. Remove scabs with wet compressed cloth
4. Consult doctor

Medications: Topical antibiotics, Antiseptics, Ointments...
Workout: Hygiene maintenance, Hydration...
Diet: Fruits, protein-rich food, vitamin C-rich meals
