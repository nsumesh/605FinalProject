# **Benchmarking Image Upscaling using GAN on CPUs and GPUs**

# **CPU Setup**
The CPU code has been written in project_cpu.ipynb. Before running any other cells, install the dependencies by running the first cell in the notebook. The model can be downloaded from the kaggle link below. For local run, note the local path to where the model is saved and change the path to the model in the 3rd cell of the notebook. Make sure to run each cell sequentially.

There are 3 approaches to the CPU implementation, highlighted by the comments in their respective cells
- Part A: default unoptimized run with default thread count - 1200 images
- Part B: default unoptimized run with multiple variable thread counts - 60 images
- Part C: OpenVINO optimized run - 1200 images

# **GPU Setup**
The GPU code has been written in project_gpu.ipynb. If you're running it locally, you will have to change the system working directory in the first block of code to add the cloned ESRGAN model to the working directory. The weight path file has to be loaded for use here. 

# **Link to ESRGAN model**
[Link](https://www.kaggle.com/models/anupsingh2510/rrdb_esrgan_x4.pth/PyTorch/default/1)
