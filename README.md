# Factual Error Correction for Abstractive Summarization Models

This directory contains code necessary to replicate the training and evaluation for the EMNLP 2020 paper ["Factual Error Correction for Abstractive Summarization Models"](https://arxiv.org/abs/2010.08712) (Meng Cao, Yue Dong, Jiapeng Wu and Jackie Chi Kit Cheung).

## Directory Structure

Our code is organized into four subdirectories:

* `build_dataset`: code for building the aritificial trianing & test dataset.
* `cnn-dailymail`: directory for the cnn-dailymail summarization dataset.
* `K2019`: directory for the manually annotated dataset by Kryscinski et al. (2019).
* `model`: wrapper for the fariseq BART model for training.

## (1) Build Dataset
To build the training dataset, first download the processed cnn-dailymail dataset from [this link](https://drive.google.com/file/d/1tqjxX5abjKOt9VS_nNiTvIGQlWl53iUm/view?usp=sharing). Unzip and save the downloaded files in `cnn-dailymail`.

Then, run the data creation bash to build the training data:

```
cd build_dataset
sh create_data.sh
```

## (2) K2019
The annotated cnn-dailymail test set from [Kryscinski et al. 2019 ACL paper](https://arxiv.org/pdf/1910.12840.pdf).
