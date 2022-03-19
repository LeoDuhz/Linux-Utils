problems with cuda

- cudnn
- https://developer.nvidia.com/rdp/cudnn-archive
sudo cp cuda/include/cudnn.h /usr/local/cuda/include/
 
sudo cp cuda/lib64/libcudnn* /usr/local/cuda/lib64/
 
sudo chmod a+r /usr/local/cuda/include/cudnn.h
 
sudo chmod a+r /usr/local/cuda/lib64/libcudnn*

- cuda path
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda/lib64
export PATH=$PATH:/usr/local/cuda/bin
export CUDA_HOME=$CUDA_HOME:/usr/local/cuda

- change cuda version
- just change the symbolic link of /usr/local/cuda
