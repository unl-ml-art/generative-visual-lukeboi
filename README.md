# Project 3 Generative Visual

Luke Farritor

## Abstract

GAN-generated heightmaps then fed into blender. see output.mp4. Heightmapts are generated by a DCGAN model trained on selections of [US topography data] (https://portal.opentopography.org/datasetMetadata?otCollectionID=OT.042013.4326.1). Dataset is not included in this repo due to size constraints.

## Model/Data

model is in ipynbs there's a train and a infer
train trains
infer makes interplations between random spots in latent space
feed interpolation images into movie (ffmpeg) and then into blender displace modifier
render blender and make movie (ffmpeg) to get output
