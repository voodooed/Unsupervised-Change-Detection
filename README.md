# Unsupervised-Change-Detection

Change detection is the process of identifying differences in land cover over time. As human
and natural forces continue to alter the landscape, it is important to develop monitoring
methods to assess and quantify these changes. Recent advances in satellite imagery, in terms
of improved spatial and temporal resolutions, are allowing for efficient identification of
change patterns and the prediction of areas of growth.

This repository will be outlining an unsupervised method for change detection. It involves the
automatic analysis of the change data, i.e. the difference image, constructed using the multi
temporal images. A difference image is the pixel-by-pixel subtraction of the 2 images. Eigen
vectors of pixel blocks from the difference image will then be extracted by Principal
Component Analysis (PCA). Subsequently, a feature vector is constructed for each pixel in
the difference image by projecting that pixel’s neighbourhood onto the Eigen vectors. The
feature vector space, which is the collection of the feature vectors for all the pixels, upon
clustering by K-means algorithm gives us two clusters – one representing pixels belonging to
the changed class, and other representing pixels belonging to the unchanged class. Each pixel
will belong to either of the clusters and hence a change map can be generated.

Automatic change detection in images of a region acquired at different times is one the most
interesting topics of image processing. Such images are known as multi temporal images.
Change detection involves the analysis of two multi temporal satellite images to find any
changes that might have occurred between the two time stamps. It is one of the major
utilization of remote sensing and finds application in a wide range of tasks like defence
inspections, deforestation assessment, land use analysis, disaster assessment and monitoring
many other environmental/man-made changes

Implemented from this 
