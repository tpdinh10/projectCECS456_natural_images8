## How to Run This Notebook

**This project is meant to run in Google Colab with a GPU.**

1. Turn on GPU in Colab

In Colab, go to:
Runtime → Change runtime type → Hardware accelerator → GPU → Save

2. Get your Kaggle API token from your profile

Go to https://www.kaggle.com/

Click your profile picture (top right)

Click Settings

Scroll down to the API section

Click Generate new token

Kaggle will show you a token string that looks like:
KGAT_abcdef123456...

Copy that whole token string

3. Paste the token into the first cell of the notebook

At the top of the notebook, find this line:

api_token = "KGAT_XXXXXXXX"


Replace the value with your real token string from Kaggle, for example:

api_token = "KGAT_b817092e5f6dd3498879d848f525d728"


4. Run all cells from top to bottom

After you paste your token:

Run each cell in order

The notebook will:

Use the Kaggle API to download the Natural Images dataset from:
https://www.kaggle.com/datasets/prasunroy/natural-images

Unzip and load the images

Build and train the ResNet50 model

Show accuracy, loss, confusion matrix, and training curves

