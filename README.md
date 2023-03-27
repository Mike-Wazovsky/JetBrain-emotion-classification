# JetBrain-emotion-classification

[Direct link on GoogleCollab](https://colab.research.google.com/github/Mike-Wazovsky/JetBrain-emotion-classification/blob/main/Jetbrains_emotion_classification.ipynb)

The solution lies in the file JetBrains_emotion_classification.ipynb

The trained model is in finalized_model.sav

Some intermediate solutions that showed the worst results I put in a folder

# Usage
To use trained model do this:

```python
# load the model from disk
loaded_model = pickle.load(open(filename, 'rb'))
result = loaded_model.predict(X_test)
```

# Result

```
              precision    recall  f1-score   support

           N       0.20      0.17      0.18        12
           O       0.67      0.68      0.68        63
           P       0.84      0.85      0.84       125

    accuracy                           0.76       200
   macro avg       0.57      0.57      0.57       200
weighted avg       0.75      0.76      0.75       200
```
