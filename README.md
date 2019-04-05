
[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/keras-team/keras/blob/master/LICENSE)

Basic workaround making Keras work with tensorflow 2.0 backend. It has marginal use since Keras is included in tensorflow 2.0 itself but with this you can run old code without changing a single line. 

If you want to replicate this with official keras, only change you have to do is to replace "import tensorflow as tf" with "import tensorflow.compat.v1" as tf, and then add the line "tf.disable_eager_execution()" everywhere in the code.

Or just install this with pip install git+https://github.com/robertofratello/keras-tensorflow2.0compat/#egg=keras (assuming you have already tensorflow 2.0).
