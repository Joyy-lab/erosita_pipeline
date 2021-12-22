# eROSITA Data Analysis Pipeline
## Introduction
Download erosita data:

cone search example: https://sciserver.mpe.mpg.de/erosita-services/conesearch/observation/get?ra=135&dec=1&r=1&runit=deg&format=json

ra, dec must in degree

Set cone radius to 0.01 and unit of arcsec. So that the target would definitely be covered.

Note that ra, dec for website have maximum four float digits.

Response:

1. No corresponding observations: 'No results in area'
2. Having observations: json file

Data reduction and analysis:
1. merge events and image file
2. source detection and catalog production
3. exposure and PSF map generation
4. light curve and spectrum extraction and analysis

## Usage
1. ./erosita\_pipeline --help to get infomation of arguments
2. ./erosita\_pipeline ra dec: Download data and run all tasks
3. ./erosita\_pipeline ra dec --without-reduction: Forbid reduction and download 
