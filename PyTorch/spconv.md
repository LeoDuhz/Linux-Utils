- spconv is a library for sparse convolution and widely used in detetcion and segmentation problems
- most of current codes use v1.2.1 not v2(there are some changes in version2 therefore codes may not work)
- usage:
git clone git@github.com:traveller59/spconv.git --recursive
git checkout v1.2.1
python setup.py bdist_wheel
cd dist
pip install *

- problems:
- about torch: after trying so many versions, the only torch version that can work is 1.4.0
- about cuda: i recommend cuda version to be 10.1 or 10.0, 11 may not work
- if you are using pytorch 1.4+ and encounter "nvcc fatal: unknown -Wall", you need to go to torch package dir and remove flags contains "-Wall" in INTERFACE_COMPILE_OPTIONS in Caffe2Targets.cmake. This problem can't be fixed in this project (to avoid this, I need to remove all torch dependency in cuda sources and drop half support).
- cannot find pybind: You may forget the --recursive in git clone;  git submodule --recursive will work

- spconv can also be installed by pip, but you will install version2
- pip install spconv-cu101
