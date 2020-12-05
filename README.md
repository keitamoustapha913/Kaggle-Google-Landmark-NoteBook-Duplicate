# Kaggle-Google-Landmark-NoteBook-Duplicate

Master AI Deep Learning Class Project : 

* Take a finished deep learning competition
* Take the code of one of the top20 participants
* Explain notebook code and concepts used


# Context of the competiton

`The Google Landmark Recognition Challenge 2020 On Kaggle`

Have you ever gone through your vacation photos and asked yourself : What was the name of that temple I visited in China ? or Who created this monument I saw in France.

Landmark Recognition can help!


## Objectif 

* The use of landmark recognition to help find and recognize landmarks from photos

* Landamrk recognition can predict landamrk labels directly from image pixels, to help people better understand and organize their photos collections.

* Challenges Kagglers to build models that recognize the correct landmark (if any ) in a dataset of challenging test images.

* Classification of 158k+ images of about 15k landmarks categories


## Challenges

* Large number of categories
* Imbalanced training set ( only a few training images for some categories)
* Very hard test set (only a fraction of images actually depict landamarks)
* GAP (Global Average Metrics) metrics (i.e confidence scores are very important)


## Datasets

### File Description

* `test/`         contains testing set of images to recognize which landamrks
* `train/`        contains training set of images with corresponding landmark labels in train.csv
* `sample_submission.csv`   A sample submission file n the correct format
* `train.csv`   corresponding landmarks labels of train set images  

### Data Description

Each image has a unique `id`. Since there are a large number of images, each image is placed within three subfolders according to the first three characters of the image `id` (i.e image `abcdef.jpg`) is placed in `a/b/c/abcdef.jpg` ).


## Notebook Used

Source code of the 7th place Team `DNA`.https://www.kaggle.com/andy2709/fork-of-recognition-notebook-16367c-511fa4-95d3bf?scriptVersionId=43685736 


### Addition Import files to Notebook 

* `superpoint-pytorch`  https://www.kaggle.com/andy2709/superpoint-pytorch
* `semantic-segmemtation-pytorch`   https://www.kaggle.com/andy2709/semantic-segmentation-pytorch/download
* `landmark-lib`    https://www.kaggle.com/andy2709/landmark-lib
* `train-embeddings`    https://www.kaggle.com/andy2709/train-embeddings

### Features Used

- `Superpoint`
- `SuperGlue for Local Re-Ranking`
