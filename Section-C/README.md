# Section C
## Image Processing

The task was to use a pair of stereo images (one left and one right) and optimize the RMSE between the two images using the disparity.
___

## Our Approach
#### Since we had limited time we used 3 images from the dataset to generate and optimize RMSE using disparity
##### Important Points 
- Basic Block matching algorithm was used
- 2 loss functions were tested SAD (sum of absolute distances) and SSD (Sum of squared distances)
- The images were tested on 2 factors - Block size and Window Size
    - 1. block size 5, window size 50
    - 2. block size 7, window size 50
    - 3. block size 10, window size 100

##### Results
- It was observed that RMSE was always reduced on using the disparity map
- However there was a mixed trend on use cases
    - On some images the RMSE increased on increasing block size from 5 to 7 but on 1 image it reduced
- Having a greater window size helped in smoothening of noise in the disparity map

#### A comparision bar graph is present at the end of each notebook

Dataset :
http://vision.middlebury.edu/stereo/submit3/

