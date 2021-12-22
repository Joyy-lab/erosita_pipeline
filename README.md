# eROSITA Data Analysis Pipeline
## Introduction
Download erosita data:

Download eROSITA Early Data Release for give R.A. and Dec in degree.

Data reduction and analysis:
1. merge events and image file
2. source detection and catalog production
3. exposure and PSF map generation
4. light curve and spectrum extraction and analysis

## Requirement
eSASS: https://erosita.mpe.mpg.de/edr/DataAnalysis/esassinstall.html

python library: astropy, scipy, numpy

You can use docker to obtain complete system: see https://hub.docker.com/r/suzhao/erpl or "docker pull suzhao/erpl:latest"

## Usage
1. ./erosita\_pipeline --help to get infomation of arguments
2. ./erosita\_pipeline ra dec: Download data and run all tasks
3. ./erosita\_pipeline ra dec --without-reduction: Forbid reduction and download 
