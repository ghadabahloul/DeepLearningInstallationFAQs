## Openpose on Fedora 25

### Main problem: 
   - Caffe links to CUDA 8.0 maximum gcc support is 5 but on Fedora 25, gcc version is 6
   - opencv version 3.1 compiled with lack of some gstreamers created big issues when run the videos
### Solutions:
   - Install gcc version 5
   - compile opencv > 3.2.0 from source:
      + install libv4l-devel:
        sudo dnf install libv4l-devel
      + activate WITH_LIBV4L=ON
   - The rest just follow the defaults installation from Openpose.
   
   
### Tips:
Always becareful with the syntax of Makefile. A litle error and nothing works.
