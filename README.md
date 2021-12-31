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
