# cvpr2023 submission
The repository contains code for CVPR 2023 paper titled - "DF-Platter: Multi-face Heterogenous Deepfake Dataset. The submission number of our paper is 10902.

## Installation
```shell
$ pip install torch
$ pip install numpy
$ pip install matplotlib
$ pip install sklearn
$ pip install tqdm
$ pip install scipy
```

## Training
```shell
$ ./train_script.sh
```
The hyperparamters like learning rate, batch size and number of epochs can be varied by making changes in the config.py file. The trained models will be saved in the saved_models folder which needs to be created in the root directory. 

## Testing
```shell
$ ./test_script.sh
```
The results are stored in a mat file inside the predictions folder which needs to be created in the root directory. The testing can be done on all the 3 sets - A,B,C by chaning the flag '--eval_set_id' in the test script.

## Evaluation
```shell
$ ./eval_script.sh
The evaluation script takes the saved mat files and outputs the results in a tabular manner. It prints out frame-level and video-level accuracy along with the AUC scores. Face-level accuracy is also printed when tested on SetB and SetC.


