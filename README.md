# Cats vs Dogs Classification (DenseNet-121)

Image classifier that tells cats from dogs, made for my AI elective. It uses transfer learning on DenseNet-121 (pretrained on ImageNet) and gets around 99% validation accuracy on the Cats vs Dogs dataset.

It builds on a basic baseline that had a few problems - the images were being normalized twice and DenseNet's own preprocessing was missing, which kept the accuracy low. Fixing those and using the pretrained features properly is what pushed it up.

## How to run

Made for Google Colab with a GPU:

1. Open the notebook in Colab
2. Runtime > Change runtime type > GPU
3. Run all the cells

Or locally:

```
pip install tensorflow tensorflow-datasets scikit-learn matplotlib
jupyter notebook
```

The dataset downloads on its own through TensorFlow Datasets, so there's nothing else to set up. The notebook includes the accuracy and loss plots and a confusion matrix on the validation set.
