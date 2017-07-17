# DeepLearningInstallationFAQs 

## Install Caffe for Openpose
Error: identifier "__float128" is undefined

Solution: 
   change suffix.hpp line 510, from
        extension typedef float128 float128_type;
    to
    __extension__ typedef long double float128_type;
    
    Ref: https://github.com/BVLC/caffe/issues/3578
