# Nihongo-MNIST 🎌
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-blue.svg)](https://creativecommons.org/licenses/by-sa/4.0/)  
## Prerequisites
```
$ pip install keras numpy matplotlib seaborn PIL
```
Otherwise, you can install Anaconda for settings environment [https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)

## The Dataset

- Kuzushiji-MNIST is a drop-in replacement for the MNIST dataset (28x28 grayscale, 70,000 images), provided in the original MNIST format as well as a NumPy format. Since MNIST restricts us to 10 classes, we chose one character to represent each of the 10 rows of Hiragana when creating Kuzushiji-MNIST.

- Kuzushiji-49 as the name suggests, has 49 classes (28x28 grayscale, 270,912 images), is a much larger, but imbalanced dataset containing 48 Hiragana characters and one Hiragana iteration mark.

- Kuzushiji-Kanji is an imbalanced dataset of total 3832 Kanji characters (64x64 grayscale, 140,426 images), ranging from 1,766 examples to only a single example per class.



### Kuzushiji-MNIST

Kuzushiji-MNIST contains 70,000 28x28 grayscale images spanning 10 classes (one from each column of [hiragana](https://upload.wikimedia.org/wikipedia/commons/thumb/2/28/Table_hiragana.svg/768px-Table_hiragana.svg.png)), and is perfectly balanced like the original MNIST dataset (6k/1k train/test for each class).

| File            | Examples | Download (MNIST format)    | Download (NumPy format)      |
|-----------------|--------------------|----------------------------|------------------------------|
| Training images | 60,000             | [train-images-idx3-ubyte.gz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/train-images-idx3-ubyte.gz) (18MB) | [kmnist-train-imgs.npz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-train-imgs.npz) (18MB)   |
| Training labels | 60,000             | [train-labels-idx1-ubyte.gz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/train-labels-idx1-ubyte.gz) (30KB) | [kmnist-train-labels.npz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-train-labels.npz) (30KB)  |
| Testing images  | 10,000             | [t10k-images-idx3-ubyte.gz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/t10k-images-idx3-ubyte.gz) (3MB) | [kmnist-test-imgs.npz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-test-imgs.npz) (3MB)   |
| Testing labels  | 10,000             | [t10k-labels-idx1-ubyte.gz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/t10k-labels-idx1-ubyte.gz) (5KB)  | [kmnist-test-labels.npz](http://codh.rois.ac.jp/kmnist/dataset/kmnist/kmnist-test-labels.npz) (5KB) |


### Kuzushiji-49

Kuzushiji-49 contains 270,912 images spanning 49 classes, and is an extension of the Kuzushiji-MNIST dataset.

| File            | Examples |  Download (NumPy format)      |
|-----------------|--------------------|----------------------------|
| Training images | 232,365            | [k49-train-imgs.npz](http://codh.rois.ac.jp/kmnist/dataset/k49/k49-train-imgs.npz) (63MB)   |
| Training labels | 232,365            | [k49-train-labels.npz](http://codh.rois.ac.jp/kmnist/dataset/k49/k49-train-labels.npz) (200KB)  |
| Testing images  | 38,547             | [k49-test-imgs.npz](http://codh.rois.ac.jp/kmnist/dataset/k49/k49-test-imgs.npz) (11MB)   |
| Testing labels  | 38,547             | [k49-test-labels.npz](http://codh.rois.ac.jp/kmnist/dataset/k49/k49-test-labels.npz) (50KB) |


### Kuzushiji-Kanji

Kuzushiji-Kanji is a large and highly imbalanced 64x64 dataset of 3832 Kanji characters, containing 140,426 images of both common and rare characters.  
The full dataset is available for download [here](http://codh.rois.ac.jp/kmnist/dataset/kkanji/kkanji.tar) (310MB).  

## License

Both the dataset itself and the contents of this repo are licensed under a permissive  [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license, except where specified within some benchmark scripts. CC BY-SA 4.0 license requires attribution, and we would suggest to use the following attribution to the KMNIST dataset.

"KMNIST Dataset" (created by CODH), adapted from "Kuzushiji Dataset" 
(created by NIJL and others), doi:10.20676/00000341
