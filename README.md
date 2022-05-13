# Project 3 Generative Visual

Luke Farritor



## Abstract

GAN-generated heightmaps then fed into blender. see output.mp4. Heightmapts are generated by a DCGAN model trained on selections of [US topography data] (https://portal.opentopography.org/datasetMetadata?otCollectionID=OT.042013.4326.1). Dataset is not included in this repo due to size constraints.

## Model/Data

download GIS data from link above, be sure to do asc format. any map selection can be used, i just drew a box over nebraska/wyoming/colorado
run dataset generation notebook to generate images usable for gan training dataset
model is in ipynbs there's a train and a infer, run both
the train notebook trains the model
infer makes interplations between random spots in latent space
feed interpolation images into movie (ffmpeg) and then into blender displace modifier
render blender and make movie (ffmpeg) to get output

note that you'll have to re-create some blender image/texture asssociations when downloading to another computer

# Interesting paper I took inspiration from
https://arxiv.org/abs/1707.03383
