# cell-growth
Tracking cell growth for individual cells from ND2 Video

## ND2 File Format
ND2 is a image file format provided from Nikon. It is not a typical file format, so it must be read in a special way. ND2 files include the following metadata:

* ```width:``` the width of the image in pixels
* ```height:``` the height of the image in pixels
* ```date:``` the date the image was taken
* ```fields_of_view:``` the fields of view in the image
* ```frames:``` a list of all frame numbers
* ```z_levels:``` the z levels in the image
* ```total_images_per_channel:``` the number of images per color channel
* ```channels:``` the color channels
* ```pixel_microns:``` the amount of microns per pixel
* ```rois:``` the regions of interest (ROIs) defined by the user
* ```experiment:``` information about the nature and timings of the ND experiment [1]

Reading in these files is not a trivial process and therefore (at least for now), I will be using a third party library. The documentation and install instructions are located [here](http://www.lighthacking.nl/nd2reader/index.html)
### References
[1] http://www.lighthacking.nl/nd2reader/index.html
