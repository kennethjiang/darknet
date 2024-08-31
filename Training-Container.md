1. Launch AWS VM using Image "amazon/Deep Learning AMI GPU CUDA 11.4.3 (Ubuntu 18.04) 20221107", or on a baremetal server with nvidia-docker2 installed
2. `docker run  -v "$(pwd):/data" --gpus all  --runtime=nvidia --rm -ti nvcr.io/nvidia/cuda:11.4.3-cudnn8-devel-ubuntu20.04 bash`
3. cd /data/ml-data/tools/darknet && make clean && make -j4
