Playing around with Keras

Some notebooks as I work out if I can do anything useful
with Keras...

Install
=======

I'm using Keras and the TensorFlow backend. It makes sense to
install this in its own environment and I'm an anaconda user and
am moving most of my python over to python 3. So the first step is
to set up a full new anaconda environment using python 3.5:

    conda create -n tensorflow python=3.5 anaconda

Then switch to the new environment:

    source activate tensorflow

The next step is to install the TensorFlow backend inside the conda 
environment following the documentation at 
https://www.tensorflow.org/install/install_mac#installing_with_anaconda
this amounts to running:

    pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-1.0.1-py3-none-any.whl

Do the basc validation by following the instructions at: https://www.tensorflow.org/install/install_mac#ValidateYourInstallation - I get warnings about
tensorflow not using SSE4.1, 4.2 AVX AVX2 and FMA instructions. But I'm only
playing on this machine so I'll take the (probably quite big) hit. Finally,
install keras:

    pip install keras

It seems this also installs the theano back end.



