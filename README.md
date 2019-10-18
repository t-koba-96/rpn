# openpose, handpose, object detection  

## setup  

First , setup the ttfnet by reading ttfnet.md.

Next, load each model from the URL and make the weights file to use them.  
Make sure the directory level and pth names are the same.

```
handpose  
  /weights 
    /openpose  
        /body_pose_model.pth
        /hand_pose_model.pth 
    /ssd
        /pretrained.pth
    /ttfnet 
        /latest.pth
```  


- Weights　URL
    - [openpose](https://www.dropbox.com/sh/7xbup2qsn7vvjxo/AABWFksdlgOMXR_r5v3RwKRYa?dl=0)
    - [ssd](https://s3.amazonaws.com/amdegroot-models/ssd300_mAP_77.43_v2.pth)  
    - [ttfnet](https://github.com/t-koba-96/rpn/releases/download/ttfnet_weight/latest.pth)



## test the demo  

make the datafile for demo inputs and outputs  

``` 
handpose  
  /demo  
    /input  
        /**.jpg  
        /**.mp4  
    /output  
```  

## testing code  

Their are two codes you can test, img_test.py and video_test.py.  
For both of them ,you can chose the openpose model or the handpose model.

For img_test.py try 

``` 
$ python img_test.py [mode(chose "handpose" or "openpose" )]
```  


For video_test.py try 

``` 
$ python video_test.py [mode(chose "handpose" or "openpose" )] [video(e.g. test.mp4 , cooking.avi)]
```  
  
