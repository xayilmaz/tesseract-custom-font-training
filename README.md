# Tesseract Training for New Fonts
## This repository has the scripts for installing and training Tesseract 4+.

### Folder Structure
The project has the following structure:

```
|-- README.md
|-- fonts                       // This is where you place the font
|-- output                      // Checkpoints and model saved here
|-- train                       // Training Data is placed here
|-- training.sh                 // Script for Training Tesseract
|-- install_tesseract.sh        // Script for installing Tesseract
```
### System Configurations
- Instance type : ```t2.large```
- Storage : ```6 GB```
- Operating System: ```Ubuntu 18.04 LTS```
### Steps for Running the Project
1. Run ```./install_tesseract.sh```
2. Run ```./training.sh```

### Tuning Parameters
Two parameters that can be tuned to increase the performance of the model are:

1. ```MAX_PAGES:``` This is the number of pages generated for training the model.
2. ```NUM_ITERATIONS:``` This is the number of times the fine-tuning process will happen.

The parameters are available in the ```training.sh``` file.