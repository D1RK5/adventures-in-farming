# adventures-in-farming

Notes for the GrainBrain: https://github.com/D1RK5/adventures-in-farming/blob/main/GrainBrain.ipynb

In order to use this, please log in/create a Google account, then go to https://colab.research.google.com/ and copy the file's GitHub URL to this input box:

![image](https://github.com/D1RK5/adventures-in-farming/assets/144019342/955288be-aa7b-4664-84b0-097b80f49c6d)

When you run the code block below, you will be asked to authenticate the Google Earth Engine. If you have never used it before, sign up; it is free. https://developers.google.com/earth-engine/guides/access#individual-signup_1

``` 
import ee
ee.Authenticate()
ee.Initialize()
``` 
     
A few caveats because they are the best. 
1. The code comes under the buy a beer and reference licence. Ie. If you find it useful, please reference me, and you now owe me one beer.
2. There is no warranty whatsoever
3. We are using composite images in order to grab the best pixels; this is useful if your farm is plagued by clouds
4. In order to get the latest images, change the second date on this line in block 52:

```
SENTINEL_COLLECTION = sc.get_collection(area, '2017-01-01','2023-08-24', 10)

```
   
