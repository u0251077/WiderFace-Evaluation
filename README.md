# WiderFace-Evaluation
Python Evaluation Code for [Wider Face Dataset](http://mmlab.ie.cuhk.edu.hk/projects/WIDERFace/)


## Usage


##### before evaluating ....

````
$ git clone https://github.com/u0251077/WiderFace-Evaluation.git
$ python3 setup.py build_ext --inplace

#requirement list
$ pip install ...
tqdm 
numpy
scipy
IPython
````
##### download_testing data 

https://drive.google.com/drive/folders/19nDDSkAga1CNFDPhM-kjx4BX5957XJrS?usp=sharing
- folder structure
```
-Widerface-Evaluation
 |-->ground_truth
 |-->pred_off_nomask
```

##### evaluating

**GroungTruth:** `wider_face_val.mat`, `wider_easy_val.mat`, `wider_medium_val.mat`,`wider_hard_val.mat`

````
$ python3 evaluation.py -p <your prediction dir> -g <groud truth dir>
````

## Bugs & Problems
please issue

## Acknowledgements

some code borrowed from Sergey Karayev
