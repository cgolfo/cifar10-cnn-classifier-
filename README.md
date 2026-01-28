# cifar10-cnn-classifier-
Deep Learning CNN for CIFAR-10 image classification using PyTorch - Achieved 68% test accuracy


Step-by-Step Guide: Running CIFAR-10 CNN on Google Colab
Prerequisites

A Google account (for Google Colab access)
A web browser
That's it! No installation needed.


Step 1: Download the Project Files

Download these files to your computer:

cifar_cnn_colab.ipynb (the main notebook)
README.md (optional - for reference)


Save them in a folder you can easily find (e.g., Desktop or Downloads)


Step 2: Open Google Colab

Open your web browser
Go to: https://colab.research.google.com/
Sign in with your Google account if prompted


Step 3: Upload the Notebook
Method A: Direct Upload

In Google Colab, click "File" in the top menu
Click "Upload notebook"
Click "Choose File" or drag and drop cifar_cnn_colab.ipynb
Wait for it to upload (should take just a few seconds)

Method B: From Google Drive (Alternative)

Upload cifar_cnn_colab.ipynb to your Google Drive
In Google Colab, click "File" → "Open notebook"
Click the "Google Drive" tab
Navigate to and select your notebook


Step 4: Enable GPU (CRITICAL for Speed!)
🚨 Important: This makes training 10-20x faster!

In the Colab notebook, click "Runtime" in the top menu
Click "Change runtime type"
A popup will appear - under "Hardware accelerator", select "GPU"
Click "Save"

You should see "GPU" or "T4" in the top-right corner now.

Step 5: Run the Notebook
Now you'll run each cell (code block) in order:
Cell 1: Import Libraries

Click on the first code cell (the one that says import torch)
Click the ▶ Play button on the left side of the cell
Wait for it to finish (you'll see a green checkmark ✓)
You should see output like: Using device: cuda

Cell 2: Define CNN Architecture

Click the play button on the next cell
Wait for the green checkmark
You'll see the model architecture printed

Cell 3: Load CIFAR-10 Dataset

Click the play button
First time only: You'll see download progress bars (about 170 MB)
This takes 1-2 minutes on first run
You'll see: Training samples: 50000 and Test samples: 10000

Cell 4: Visualize Sample Images

Click play
You'll see 8 random images from the dataset with labels
Great! Now you know what the data looks like

Cell 5: Setup Training

Click play
Quick setup - should finish in 1 second
Shows optimizer and loss function info

Cell 6: Train the Model ⏱️
This is the main step - takes about 15-20 minutes

Click play
You'll see training progress like:

   Epoch [1/10], Step [100/782], Loss: 1.5234
   Epoch [1/10], Step [200/782], Loss: 1.3456
   ...
   Epoch [1/10] - Training Accuracy: 45.23%

Don't close the browser tab - Colab will stop training
You can minimize it and do other things
All 10 epochs will complete automatically

Cell 7: Evaluate the Model

Click play after training finishes
You'll see:

Overall test accuracy (should be 65-75%)
Per-class accuracy for each of the 10 classes



Cell 8: Visualize Predictions

Click play
You'll see 8 test images with:

Green text = correct prediction
Red text = incorrect prediction


Shows "True: [actual class]" and "Pred: [predicted class]"

Cell 9: Save the Model

Click play
Model saved as cifar_cnn_model.pth
You can download it by uncommenting and running the download lines

