# Weather Prediction using Naive Bayes

This project demonstrates how to apply a **Naive Bayes classifier** to predict whether a game will be played based on weather conditions. The dataset includes features such as Outlook, Temperature, Humidity, and Windy conditions, with the target label being whether a game is played (`Play`).


## Naive Bayes Algorithm

**Naive Bayes** is a probabilistic classification algorithm based on Bayes' theorem, assuming that the features are conditionally independent. It works well for categorical input variables and is often used in text classification problems.

For weather prediction, we assume that the probability of a game being played (`Play = yes` or `no`) is influenced by weather conditions like `Outlook`, `Temperature`, `Humidity`, and `Windy`.

### Gaussian Naive Bayes

We use **Gaussian Naive Bayes** since some of our features (like Temperature) might be numerical. Gaussian Naive Bayes assumes that features follow a normal distribution.

The algorithm steps are as follows:

1. **Encode categorical variables** using `LabelEncoder` to convert them into numerical values.
2. **Train the Naive Bayes model** using the weather data.
3. **Make predictions** for new weather data points.
4. **Evaluate the model** using accuracy and confusion matrix.


Additionally, the model predicts the outcome for a new weather condition (Rainy, Hot, High Humidity, No Windy) as:
```
Predicted outcome: no
```

## Conclusion

The Naive Bayes classifier is simple yet effective for weather prediction problems. By using Gaussian Naive Bayes, we were able to model the relationship between weather conditions and game outcomes.

In future iterations, we could explore additional techniques to improve model accuracy, such as:
- Tuning hyperparameters.
- Collecting a larger and more balanced dataset.
- Experimenting with different types of Naive Bayes models.
