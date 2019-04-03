# Keras: Deep Learning for humans

![Keras logo](https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png)

[![Build Status](https://travis-ci.org/keras-team/keras.svg?branch=master)](https://travis-ci.org/keras-team/keras)
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/keras-team/keras/blob/master/LICENSE)

Basic workaround making Keras work with tensorflow 2.0 backend. It has marginal use since Keras is included in tensorflow 2.0 itself but with this you can run old code without changing a single line. 

If you want to replicate this with official keras, only change you have to do is in \keras\backend\tensorflow_backend.py

You have to change on line 5 "import tensorflow as tf" with "import tensorflow.compat.v1" as tf, and then add the line "tf.disable_eager_execution()"

Or just install this with pip install git+https://github.com/robertofratello/keras-tensorflow2.0compat/#egg=keras (assuming you have already tensorflow 2.0 installed).
