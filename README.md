# Transfer-learning-for-classification-of-cats-and-dogs
use transfer learning for kaggle cats_vs_dogs

---
# How it works
first using ResNet50 to extract features from data and store in features.hdf5 file.Then create logistic regression classifier to classify cats and dogs

---
# Dependency
1. keras
2. scikit-learn
3. h5py
4. imutils
5. numpy
6. progressbar

---
# How to run 
first run `extract_features.py` using following command
`python extract_features.py --dataset datasets/train --output datasets/features.hdf5`

it will create file name `features.hdf5` inside hdf5 folder

then run `train_model.py` using following command
`python train_model.py --dataset datasets/features.hdf5 --model datasets/dogs_vs_cats.pickle`
