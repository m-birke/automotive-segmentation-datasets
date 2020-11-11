# Playing for Data

Extracted from Grand Thef Auto 5 (GTA)

__Image Dimensions:__

* ~5000 images with 1046x1914
* ~20000 images with 1052x1914

__Outlier:__ 15617.png has only one class label in the whole image

## Corrupt data

The corresponding labels to the following 60 images have other dimensions than the images themself:

20805.png, 20857.png, 20823.png, 20821.png, 20841.png, 20853.png, 20829.png, 20855.png, 20849.png, 20838.png, 20806.png, 20814.png, 20815.png, 20816.png, 20844.png, 20828.png, 20845.png, 20827.png, 20820.png, 20847.png, 20839.png, 20817.png, 20833.png, 20809.png, 20830.png, 20803.png, 20807.png, 20822.png, 20842.png, 20851.png, 20819.png, 20858.png, 20810.png, 20804.png, 20859.png, 20843.png, 20854.png, 20848.png, 20836.png, 20856.png, 20834.png, 20840.png, 20825.png, 20813.png, 20846.png, 20832.png, 20852.png, 20860.png, 20826.png, 20824.png, 20801.png, 20831.png, 20835.png, 20808.png, 20850.png, 20837.png, 20818.png, 20811.png, 20802.png, 20812.png

The following two images are unusable:

1. 15188.png totally white image with dims 957x526
1. 17705.png totally black image with dims 957x526


## Classes

Number of classes: 30 (Since the labels are RGB, classes with the same color cannot be differentiated)

| Class                       | ID |             RGB | same color | pixel-wise occ [%] |
|                    ---------|----|             ----|     -------|               -----|
|'unlabeled'                  | 0  | [0,0,0]         |          X |                 8.1|
|('ego vehicle')              | 1  | [0,0,0]         |          X |                   0|
|('rectification border')     | 2  | [0,0,0]         |          X |                   0|
|('out of roi')               | 3  | [0,0,0]         |          X |                   0|
|'static'                     | 4  | [20,20,20]      |            |              0.1689|
|'dynamic'                    | 5  | [111,74,0]      |            |              1.7172|
|'ground'                     | 6  | [81,0,81]       |            |              0.3171|
|'road'                       | 7  | [128,64,128]    |            |             32.1046|
|'sidewalk'                   | 8  | [244,35,232]    |            |              8.2764|
|'parking'                    | 9  | [250,170,160]   |            |                   0|
|'rail track'                 | 10 | [230,150,140]   |            |                   0|
|'building'                   | 11 | [70,70,70]      |            |                16.9|
|'wall'                       | 12 | [102,102,156]   |            |              1.8435|
|'fence'                      | 13 | [190,153,153]   |            |              0.6331|
|'guard rail'                 | 14 | [180,165,180]   |            |              0.0249|
|'bridge'                     | 15 | [150,100,100]   |            |              0.7803|
|'tunnel'                     | 16 | [150,120,90]    |            |              0.0932|
|'pole'                       | 17 | [153,153,153]   |          P |                1.06|
|('polegroup')                | 18 | [153,153,153]   |          P |                   0|
|'traffic light'              | 19 | [250,170,30]    |            |              0.1342|
|'traffic sign'               | 20 | [220,220,0]     |            |              0.0807|
|'vegetation'                 | 21 | [107,142,35]    |            |                 7.6|
|'terrain'                    | 22 | [152,251,152]   |            |                 2.2|
|'sky'                        | 23 | [70,130,180]    |            |                13.5|
|'person'                     | 24 | [220,20,60]     |            |               0.362|
|'rider'                      | 25 | [255,0,0]       |            |               0.031|
|'car'                        | 26 | [0,0,142]       |            |              2.5154|
|'truck'                      | 27 | [0,0,70]        |            |               1.129|
|'bus'                        | 28 | [0,60,100]      |            |              0.3680|
|'caravan'                    | 29 | [0,0,90]        |            |                   0|
|'trailer'                    | 30 | [0,0,110]       |            |              0.0122|
|'train'                      | 31 | [0,80,100]      |            |              0.0648|
|'motorcycle'                 | 32 | [0,0,230]       |            |              0.0315|
|'bicycle'                    | 33 | [119,11,32]     |            |              0.0054|
