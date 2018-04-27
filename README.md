# dl-gpu
Personal docker image for deep learning

Based on https://github.com/ufoym/deepo#GPU

Install:
- https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce
- https://github.com/NVIDIA/nvidia-docker

Or check: https://medium.com/google-cloud/jupyter-tensorflow-nvidia-gpu-docker-google-compute-engine-4a146f085f17

To use this Dockerfile without having to install docker-compose on the server:
- sudo docker pull laurentvw/dl-gpu
- sudo nvidia-docker run -it -p 8888:8888 -v /notebook:/notebook laurentvw/dl-gpu jupyter notebook --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --notebook-dir='/notebook'

