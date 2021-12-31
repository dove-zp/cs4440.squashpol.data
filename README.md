
# CS 4440/5440: Artificial Intelligence, Fall 2021
## Squash Pollination - Data

Squash plants represent a half billion dollar crop in the United States and require pollinators (such as
bees) to transfer pollen from male to female flowers. Large commercial farms lease beehives by the
truckload to pollinate their crop. The placement of these hives and the lease duration are parameters
that can be optimized to maximize profit. In order to study the relationship between hive placement
and the time it takes to pollinate the crop, researchers have positioned cameras that record the
activity at several squash flowers.

Your team has been selected by the United States Department of Agriculture (USDA) to investigate
deep learning methods for detecting bee interactions with squash flowers, including ways to measure
their effectiveness. You are expected to build a deep learning model that classifies squash images
according to whether or not a bee is actively interacting with the flower and predict its effectiveness
on future images. The USDA has provided a training set of 25 flowers with 20 images showing
interactions and 20 images without, as well as a validation set of 10 flowers. 

## Evaluation

The USDA is interested in the effectiveness of deep learning for measuring the amount of time a bee is
interacting with each flower. Although the data provided is approximately equally divided between
positive and negative examples, in practice the vast majority of images will not show an interaction
with a bee. The USDA estimates that over 90% of the images collected in the future will not show an
interaction. 

## Data

### Non-Labeled

* [unsorted](https://github.com/dove-zp/cs4440.squashpol.data/tree/unsorted)
  * Raw data with no labels, filtering, and setup applied 

* [sorted](https://github.com/dove-zp/cs4440.squashpol.data/tree/sorted)
  * 35 groups of flowers with no labels applied 

### Provided

* [provided](https://github.com/dove-zp/cs4440.squashpol.data/tree/provided)
  * Provided data that comes with a preset train and valid configuration
    * Contains false-negatives and false-positives
  * Contains labels: 0, 1
  * Contains setup: train, valid

* [raw](https://github.com/dove-zp/cs4440.squashpol.data/tree/raw)
  * Data extracted from the given provided branch but into one folder for less bias
    * Contains false-negatives and false-positives
  * Contains labels: 0, 1

### Corrected

* [fixed](https://github.com/dove-zp/cs4440.squashpol.data/tree/fixed)
  * Filtered data of raw that places mislabeled images into their correct folders
    * Contains no false-negatives and no false-positives
  * Contains labels: 0, 1

### Outliers

* [light](https://github.com/dove-zp/cs4440.squashpol.data/tree/light)
  * Cleaned data of filtered that shows only "too light" closeup images of flowers
    * Contains no false-negatives and no false-positives
  * Contains labels: 0, 1

* [dark](https://github.com/dove-zp/cs4440.squashpol.data/tree/dark)
  * Cleaned data of filtered that shows only "too dark" closeup images of flowers
    * Contains no false-negatives and no false-positives
  * Contains labels: 0, 1

* [faraway](https://github.com/dove-zp/cs4440.squashpol.data/tree/faraway)
  * Cleaned data of filtered that shows only "far away" images of flowers
    * Contains no false-negatives and no false-positives
  * Contains labels: 0, 1

* [closeup](https://github.com/dove-zp/cs4440.squashpol.data/tree/closeup)
  * Cleaned data of filtered that removes "far away" images of flowers
    * Contains no false-negatives and no false-positives
  * Contains labels: 0, 1

### Normalized

* [normalized](https://github.com/dove-zp/cs4440.squashpol.data/tree/normalized)
  * Cleaned data of filtered that shows only closeup images of flowers and removes "too dark" and "too light" 
    * Contains no false-negatives and no false-positives
  * Contains labels: 0, 1

### Valid 

* [full](https://github.com/dove-zp/cs4440.squashpol.data/tree/full)
  * Full images of bees on images of flowers 
    * Contains no false-negatives and no false-positives
  * Contains labels: 1 

* [partial](https://github.com/dove-zp/cs4440.squashpol.data/tree/partial)
  * Partial images of bees on images of flowers that are easy to spot pollinating
    * Contains no false-negatives and no false-positives
  * Contains labels: 1

<!--  -->

## Feedback

I welcome your constructive input - both negative and positive. I will continue to try to provide updates when able. At some point you may find errors, inconsistencies, or methods that could be improved, or are missing altogether. Your feedback is critical to help improve future revisions.

The best way to reach out is by opening a new issue in this repository:

https://github.com/dove-zp/cs4440.squashpol.data/issues

Please be sure to refer to what your situation is when giving feedback and if possible link the topic in question.

Many thanks.

<hr/>

<p align="center">
  <p align="center">
    <a href="https://hits.seeyoufarm.com/api/count/graph/dailyhits.svg?url=https://github.com/dove-zp/cs4440.squashpol.data">
      <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdove-zp%2Fcs4440.squashpol.data&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true" alt="repository hits">
    </a>
    <a href="https://github.com/dove-zp/cs4440.squashpol.data/releases">
      <img src="https://img.shields.io/github/downloads/dove-zp/cs4440.squashpol.data/total?style=flat-square" alt="downloads"/>
    </a>
    <a href="https://github.com/dove-zp/cs4440.squashpol.data/graphs/contributors">
      <img src="https://img.shields.io/github/contributors/dove-zp/cs4440.squashpol.data?style=flat-square" alt="contributors"/>
    </a>
    <a href="https://github.com/dove-zp/cs4440.squashpol.data/watchers">
      <img src="https://img.shields.io/github/watchers/dove-zp/cs4440.squashpol.data?style=flat-square" alt="watchers"/>
    </a>
    <a href="https://github.com/dove-zp/cs4440.squashpol.data/stargazers">
      <img src="https://img.shields.io/github/stars/dove-zp/cs4440.squashpol.data?style=flat-square" alt="stars"/>
    </a>
    <a href="https://github.com/dove-zp/cs4440.squashpol.data/network/members">
      <img src="https://img.shields.io/github/forks/dove-zp/cs4440.squashpol.data?style=flat-square" alt="forks"/>
    </a>
  </p>
</p>

<p align="center">
  <a href="https://github.com/dove-zp">
    <img width="64" heigth="64" src="https://avatars.githubusercontent.com/u/89095890" alt="dove-zp"/>
  </a>  
</p>
