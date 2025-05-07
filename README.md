# Application 2 -> Image Segmentation
# 1. Measure the presence of vegetation (forest areas) in the satelite images (.jpg or .png) for the years 1985 | 1993 | 2001 | 2011.

# 2. Analysis the vegatation understanding the image's pixel values through HSV channel and and compare the RGB type image's result with HSV type channel image.

Libraries - cv2, numpy, matplotlib

Language - Python

Topics - HSV channel, Histogram (Linear and Log scale), Inrange mask, Image segmenation

Pipeline -

    > Read the images
  
    > Pre-processing :-
  
        * Convert the image of each years into HSV channel.
  
        * Split the each images into three channels - H S V
        
        * Plot the histogram of each year of images and using histogram, analysis the image - select the range of pixels whose intensities are at the highest peak in each channel.
        
        * Set the lower and upper values using histogram, which will be used while forming the mask.
        
    > Pass the origional (HSV image) image of each years into the inrange function by setting the lower and upper value (as per the image).
   
    > Post-processing :-
   
        * calculate the green part by calculating the number of pixels that are non-zero (255=white).

Result -

  > The percentage of vegetation of each years from RGB channel is different from HSV channel images.
 
  > From RGB the values are higher than from HSV, thus analysis the deforestation or any images using HSV channel of image gives accurate results as HSV splits the images into Hue, saturation and values (each color accurately distributes in each channel). 
