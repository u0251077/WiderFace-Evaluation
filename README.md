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
##### input&output
- input：
31_Waiter_Waitress_Waiter_Waitress_31_188.jpg
![](https://i.imgur.com/3kvObTC.jpg)

- output：
31_Waiter_Waitress_Waiter_Waitress_31_188.txt

```
31_Waiter_Waitress_Waiter_Waitress_31_188
2
303.0 233.0 96.0 125.0 0.9996455907821655
572.0 359.0 93.0 122.0 0.9993485808372498
```

- output explanation
```
file_name
face_numbers
(1st)x_start y_start height width prob.
(n-th)x_start y_start height width prob.
...

```

## Bugs & Problems
please issue

## Acknowledgements

some code borrowed from Sergey Karayev
