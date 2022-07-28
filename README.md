# COVID-19-Genome-Sequencing-with-DeepGRU
This was a test/proof of concept project that I wrote up for a class that I took during CAP 6545: Machine Learning for Biomedical Data under Dr. Haiyan Nancy Hu. 


## Context 

With COVID-19 in the rise during the time period that I was taking this course, I had the idea of taking a previously tested algorithm from gesture recognition and attempt to adapt it towards use with genome sequencing. This concept appealed to me since the idea of matching genome sequences was similar to that of gesture recognition in which despite having a pattern, we have to roughly estimate the data that comes in as a potential goal with that of random data. 

## Dependencies

DeepGRU requires the following dependencies

- Python v3.5+
- [PyTorch v1.2+](https://pytorch.org/)
- [Numpy](https://numpy.org/) (will be installed along PyTorch)
- (Optional) [CUDA toolkit](https://developer.nvidia.com/cuda-toolkit) with an NVIDIA GPU (for faster training, although CPU-only training still works)

Basically if you follow the instructions for the original (DeepGRU)[https://github.com/Maghoumi/DeepGRU], you should be covered for dependencies. 

## How to use?

Open a Conda or Python Environment with the respective dependencies installed. Procced with these instructions afterwards: 

`git clone https://github.com/OvercodedStack/COVID-19-Genome-Sequencing-with-DeepGRU`
`cd COVID-19-Genome-Sequencing-with-DeepGRU`
`jupyter bio_analysis_matcher.ipynb`

Once in the environment just press run in the notebook.

## How to change the training data?

By old design, I used the MLDSP_GUI_DATA folder to control the data. The independent Datasets folder is a default folder with a lot of datasets originating from the original dataset source. The Tests folder is a folder containing the 


## Licenses 

The code is provided as-is under an MIT license, which was part of DeepGRU as well. Please feel free to fork and follow code as you wish 

## Credits

Credit to Mehran Maghoumi for DeepGRU, Austin Mathews for some early ideas on getting this to run. I wrote most of the Bio_analysis_matcher.ipynb file and altered some files to get the code to work. 
