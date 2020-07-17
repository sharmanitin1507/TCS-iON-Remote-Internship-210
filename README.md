# TCS-iON-Remote-Internship-210
## Project Work.
- **Name:** NITIN SHARMA
- **Institute:** Amity University Noida, Uttar Pradesh.
- **Project Title:** Automate identification and recognition of handwritten text from an image.
## Getting Started
To run the project on your local machine, you will require the exact build of packages as some of the functions used in this project work only on these builds and are updated/removed in latest builds.
### Prerequsites
1. Install [Python 3.7.6.](https://www.python.org/downloads/release/python-376/)
2. Add Python 3.7.6 to PATH.
3. Install [PyCharm IDE Community Version.](https://www.jetbrains.com/pycharm/download/#section=windows)
4. Add launcher directory to PATH during installation.
5. Create a blank project with base interpreter. `Python37/python.exe`
### Packages
```

- Keras                 2.3.1
- matplotlib            3.1.3
- numpy                 1.18.1
- opencv-python         4.2.0.32
- sklearn               0.0
- tensorflow            2.0.0
```

### Instructions
1. Download [File1 Code.py](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/File1%20Code.py) , [File2 Code.py](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/File2%20Code.py) and [TestData.zip](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/TestData.zip) available in the [repo.](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210)
2. Add them to your project directory.
3. Execute [File1 Code.py](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/File1%20Code.py)
4. Execute [File2 Code.py](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/File2%20Code.py)
5. Use your webcam to test the digits.
## Results
After executing [File1 Code.py](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/File1%20Code.py), the result of your model can be seen as follows:
```
Model: "sequential_1"

___________________________________________________________________________________________________________________________________
Layer (type)                       Output Shape                              Param #
===================================================================================================================================
conv2d_1 (Conv2D)                  (None, 28, 28, 60)                        1560
___________________________________________________________________________________________________________________________________
conv2d_2 (Conv2D)                  (None, 24, 24, 60)                        90060
___________________________________________________________________________________________________________________________________
max_pooling2d_1 (MaxPooling2       (None, 12, 12, 60)                        0
___________________________________________________________________________________________________________________________________
conv2d_3 (Conv2D)                  (None, 10, 10, 30)                        16230
___________________________________________________________________________________________________________________________________
conv2D_4 (Conv2D)                  (None, 8, 8, 30)                          8130
___________________________________________________________________________________________________________________________________
max_pooling2d_2 (MaxPooling2       (None, 4, 4, 30)                          0
___________________________________________________________________________________________________________________________________
dropout_1 (Dropout)                (None, 4, 4, 30)                          0
___________________________________________________________________________________________________________________________________
flatten_1 (Flatten)                (None, 480)                               0
___________________________________________________________________________________________________________________________________
dense_1 (Dense)                    (None, 500)                               240500
___________________________________________________________________________________________________________________________________
dropout_2 (Dropout)                (None, 500)                               0
___________________________________________________________________________________________________________________________________
dense_2 (Dense)                    (None, 10)                                5010
===================================================================================================================================
Total params: 361,490
Trainable params: 361,490
Non-trainable params: 0
```
The accuracy of the trained model can be checked from console:
```
Test Score = 0.003487161887470976
Test Accuracy = 0.999015748500824
```
Finally, [File2 Code.py](https://github.com/sharmanitin1507/TCS-iON-Remote-Internship-210/blob/master/File2%20Code.py) is executed to test the model with new examples.

