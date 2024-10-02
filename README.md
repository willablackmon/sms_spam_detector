# sms_spam_detector

## Gradio SMS Classification Function Powered by a Support Vector Classification (SVC) Model

### Description:

Develop a Gradio applcation powered by a Support Vector Classification (SVC) model that will provide feedback to users, indicating whether entered text is classified as spam.

### Goals:

Refactor code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model.

Create a Gradio app to host the application, enabling users to test text messages. 

### Data:

Git Repo: sms_spam_detector

### Steps:

Refactor `sms_classification` function

- Set `features` to the text message column of the DataFrame.
- Set `target` to the "label" column of the DataFrame.
- Split data into training and testing with `test_size` set to 33%.
- Build a pipeline to transform the test set to compare to the training set.
- Fit the model to the transformed training data and return the model.

1. Load `SMSSpamCollection.csv` into a DataFrame and call the `sms_classification` function with the DataFrame, setting the result to the `text_clf` variable.

### Create the SMS Prediction Function

1. Use the `sms_prediction` function to predict the classification of a new text:
   - Create a variable to hold the prediction of a new text.
   - Use a conditional statement to determine if the text message is "ham" or "spam".
   - Return a message indicating whether the text is spam or not.

### Create the Gradio Interface Application

1. Create a Gradio Interface application with:
   - A textbox for inputs.
   - A textbox for outputs.
   - Labels describing each textbox.
2. Launch the application and provide the URL to share the application.


```markdown

```
