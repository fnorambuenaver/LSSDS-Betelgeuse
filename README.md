# LSSDS-Betelgeuse
Classifying Radio Signals from SETI - Project LSSDS 

### Installing Tensorflow and Packages
There's created a virtual environment from the book 'Hands on Machine Learning' from Aurelien Geron, having one shared environment allow's for programmatic development and testing. Run in command line:

```bash
conda env create -f environment.yml
```

Then to activate it
```bash
conda activate radio
```


### Folder Structure
- 0_papers
    - useful papers for the work
- 1_ninas_guide
    - contains a notebook example with a CNN implementation
- 2_fourier transform
    - contains useful guides and scripts about this algorithm
- 3_cnn
    - useful guides for convolucional neural networks
- dataset
    - contains `train` and `validation`; this file must be downloaded from:
        [download dataset](https://drive.google.com/drive/folders/15atFHE9NHiuc5oyxUynh8z6C7YI9gJF9?usp=sharing)

### Mile Stones
- [ ] Data augmentation using ImageDataGenerator
- [ ] Way of saving the weights of a model at some interval which can later be used for transfer learning through 'callbacks' during fitting the model
