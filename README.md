# picture-compare-API-log

#new potentail ones to look at
-https://www.npmjs.com/package/pixelmatch

### Notes on exploring APIs that involved comparing photos
## How to run the tested files

-Go to the coded files 
  -if it is .js 
  ```
  node filename.js
  ```
  
  -if it is .py
  ```
  python filename.py
  ```
  
  -modify the photo if you like


## 1.deepAI

https://deepai.org/machine-learning-model/image-similarity

-requires a API key

-It can compare the similarity between two photos with a return value in int. If the two pictures are exactly the same, it will return 0. If they are different, then the returned value will be bigger. The larger the value, the bigger the differences present in two photos.

-More durable than number 2 because it can take in both local files, or picture urls. However, the testing code will be different in that case.

-Tested

-Sample Results: 

```
{'id': '4dscb8b2-86bd-421e-b6da-951e8b60dbc0', 'output': {'distance': 24}}
```

## 2.Image Compare API

https://github.com/htmlcsstoimage/image-compare-api

-no API key needed

-only takes in picture urls 

-It can compare pictures pixels by pixels

-It will return an object with the data type and size for each photo, the total number of differences in pixels, and the percent difference. 

-not as useful because facial recognition requires more than just comparing pixels by pixels

-Tested

-Sample Results:

```
{'image': {'height': 3744, 'width': 5616, 'type': 'jpg'}, 'other_image': {'height': 3744, 'width': 5616, 'type': 'jpg'}, 'pixel_difference': 181686, 'percent_difference': 0.9}
```

