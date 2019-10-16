# openpose, handpose, object detection  

## load model  

load each model from the URL and make the weights file to use them.  
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
    - [ttfnet]()



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

## load model