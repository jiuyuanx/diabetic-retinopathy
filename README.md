This repository contains the resources for the explainability homework.

# The Use Case: Blindness Detection 
The use case is to detect diabetic retinopathy to stop blindness before it's too late. Consider you are building a smartphone app that could be used by end users to self-diagnose potential problems simply by looking into the smart phone's camera. Deploying such medical diagnoistics as a smart phone app has the potential to drastically reduce screening costs and make screenings much more available, especially in underresourced regions of the world. The app would provide information about a potential risk and encourage the user to get in contact with medical professionals for testing and potential treatment. In this assignment, you will focus on the model, but also consider its integration into a smartphone app.

You are provided with a large set of retina images taken using fundus photography under a variety of imaging conditions.
A clinician has rated each image for the severity of diabetic retinopathy on a scale of 0 to 4:

```
0 - No DR
1 - Mild
2 - Moderate
3 - Severe
4 - Proliferative DR
```

Like any real-world data set, you will encounter noise in both the images and labels. 
For details, you can check this [Kaggle competition](https://www.kaggle.com/c/aptos2019-blindness-detection/overview).

A `ResNet50` model is trained using this data for the classification task.

# Model and Data
The pre-trained model and data are available in this [Google Drive](https://drive.google.com/drive/folders/1X_tTwEixtZdkVWrCae3LK7maP6m2wF4T?usp=drive_link).

# Notebooks
This repository contains two notebooks. 

The training notebook is used for training the model. This is for reference. <ins>You do not need to run this notebook</ins>. You can simply download the pre-trained model from the provided link above.

There is a playground notebook that shows how to load the model and get the predictions. You can use this notebook or your own, however, you are comfortable with.

# Generating Explanation
To comply with the provided policy, you may want to generate some explanations to understand or explain the behavior of the model.

We recommend using the [Alibi Explain](https://docs.seldon.io/projects/alibi/en/stable/index.html) library. This contains many [algorithms](https://docs.seldon.io/projects/alibi/en/stable/overview/algorithms.html) that support generating explanations for classification models with image data.

You are free to use this library, any other library, or anything you are comfortable with.
