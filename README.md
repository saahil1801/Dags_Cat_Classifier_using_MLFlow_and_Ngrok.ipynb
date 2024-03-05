# Dogs_Cat_Classifier_using_MLFlow_and_Ngrok.ipynb

# Cat-Dog Classifier using MobileNet

This repository contains code for building a cat-dog classifier using the MobileNet architecture, along with instructions for setting up the environment and deploying the model to production.

## Dependencies

Before running the code, ensure you have installed the following Python packages:

```
!pip install bing-image-downloader
!pip install pyngrok
!pip install mlflow
```

## Data Collection

We utilize the Bing Image Downloader to collect images of cats and dogs for training the classifier. The code provided in the repository downloads 200 images each of cats and dogs.

```python
download_images("cat", 200, image_path)
download_images("dog", 200, image_path)
```

## Preprocessing

The collected images undergo preprocessing steps, including resizing and filtering out unsupported image formats.

## Model Training

The classifier is built using the MobileNet architecture pre-trained on ImageNet. It is fine-tuned on the collected cat-dog dataset. The training process is logged using MLflow.

## Model Evaluation

The trained model's performance is evaluated on a validation dataset, and relevant metrics are logged using MLflow.

## Deployment to Production

Once the model is trained and evaluated, it can be deployed to production. The repository provides scripts to register the model and transition it to the production stage using MLflow.

## Credits


Feel free to explore the code, experiment with different architectures, and contribute to further improvements!

Happy coding! 🚀
