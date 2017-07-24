## Caffe installation

### Fedora 25
    dnf copr enable leebc/compat-gcc-5 // activate
    dnf install compat-gcc-5
    
    
### Error with boost + CUDA 8 + CUdnn

    Error:
       /usr/include/boost/type_traits/is_floating_point.hpp(25): error: identifier "__float128" is undefined

       /usr/include/boost/type_traits/type_with_alignment.hpp(48): error: identifier "__float128" is undefined

    Change according to this link: https://github.com/boostorg/config/pull/83/files
