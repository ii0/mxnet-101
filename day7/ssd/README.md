## How to deploy this model to video

 1. **Convert model to deploy mode**
 This simply removes all loss layers, and attach a layer for merging results and non-maximum suppression.
Useful when loading python symbol is not available.

    # cd /path/to/mxnet/example/ssd
    python deploy.py --num-class 20
 2. Run the `demo_video.py`

    python demo_video_1.py --video-file=1.m4v --save-video=1_output.avi

Here is the video example in YOUTUBE

[The result video of ssd in mxnet ](https://www.youtube.com/watch?v=u1w8Re-tU0g&feature=youtu.be)