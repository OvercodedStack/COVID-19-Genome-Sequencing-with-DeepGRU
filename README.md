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

```bash
git clone https://github.com/OvercodedStack/COVID-19-Genome-Sequencing-with-DeepGRU 
cd COVID-19-Genome-Sequencing-with-DeepGRU
jupyter bio_analysis_matcher.ipynb
```
When inside the notebook please note the line 6 in block 3 and line 9 in block 4; which may cause an error if not set to the proper directory. 


Once in the environment just press run in the notebook. 

Most of the code will be readable, although some concepts will likely be needing additional reading such as one-hot encoding, genome sequencing, tensors, etc. Please do not take most of the results to heart as some of the results may be overfitting and require additional tweaking to result in functional results in my opinion. 

## How to change the training data?

By old design, I used the MLDSP_GUI_DATA folder to control the data flow. The independent `Datasets` folder is a default folder with a lot of datasets originating from the original dataset source from DeepGRU. 

The `Tests` folder is a folder containing the data as organized by Randhawa's paper with associated genome data. The data has already been organized as closely as possible to the original paper and ready to run if the user has already set this. 

For additional details, please refer to the final report pdf. Some results in that report were created by altering the code in a non-documented fashion, but it could possibly be replicable if a user can figure it out. 

## Citations and notes

This work is not under any specified grant or paper. This was simply a course assignment final project. Users may be encouraged to utilize this code for other applications but please do not reutilize this code for taking the course. I encourage users to find other techniques for implementing rather that just this project. After all, the core application of this code has almost past its importance at this point in time with newer code-bases and applications. 

## Licenses 

The code is provided as-is under an MIT license, which was part of DeepGRU as well. Please feel free to fork and follow code as you wish. 

## Credits

Credit to Mehran Maghoumi for DeepGRU, Austin Mathews for some early ideas on getting this to run. I wrote most of the Bio_analysis_matcher.ipynb file and altered some files to get the code to work. The data coming for the genomes is sourced from the NCBI website. Please visit the NCBI to adquire the most recent data for genomes at https://www.ncbi.nlm.nih.gov/
