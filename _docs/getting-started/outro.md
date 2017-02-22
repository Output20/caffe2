
| Caffe2 Python
----|-----
Module not found | Verify that Caffe2 was installed correctly
Solution | Run the following: `python -c 'from caffe2.python import core' 2>/dev/null && echo "Success" || echo "Failure"` An output of `Success` means you are ready to with Caffe2 - congratulations! An output of `Failure` usually means you have not installed one of the dependencies correctly.
Dependencies missing | It's possible you're trying to run something that was using an optional dependency.
Solution | `sudo pip install setuptools flask jupyter matplotlib scipy pydot tornado python-nvd3 scikit-image pyyaml`
matplotlib error | Sometimes you need setuptools first: `sudo pip install -U pip setuptools && sudo pip install matplotlib`

| System Dependencies
----|-----
[Nvidia CUDA 6.5 or greater](https://developer.nvidia.com/cuda-zone) |
[C++ 11](https://en.wikipedia.org/wiki/C%2B%2B11) |
[Google Protocol Buffers](https://developers.google.com/protocol-buffers/) |
[Google Logging Module](https://github.com/google/glog) |
[gflags](https://gflags.github.io/gflags/) |
[Eigen 3](http://eigen.tuxfamily.org/) |
[NumPy](http://www.numpy.org/) |

| Optional System Dependencies
----|-----
Strictly speaking, you now have everything you need to run the core Caffe2 successfully. However, for real-world deep learning (e.g., image processing, mathematical operations, etc), there are other dependencies that you will want to install in order to experience the full features of Caffe2. |
[OpenCV](http://opencv.org/) for image-related operations. |
[OpenMPI](http://www.open-mpi.org/) for MPI-related Caffe2 operators. |
[RocksdB](http://rocksdb.org) for Caffe2's RocksDB IO backend. |
[ZeroMQ](http://zeromq.org/), needed for Caffe2's ZmqDB IO backend (serving data through a socket). |
[cuDNN](https://developer.nvidia.com/cudnn), if using GPU, this is needed for Caffe2's cuDNN operators. |

| Python Optional Dependencies
----|-----
There are also various Python libraries that will be valuable in your experience with Caffe2. Many of these are required to run the tutorials. |
[Flask](http://flask.pocoo.org/) |
[Jupyter](https://ipython.org/) for the Jupyter Notebook |
[Matplotlib](http://matplotlib.org/) |
[Pydot](https://pypi.python.org/pypi/pydot) |
[Python-nvd3](https://pypi.python.org/pypi/python-nvd3/) |
[SciPy](https://www.scipy.org/) |
[Tornado](http://www.tornadoweb.org/en/stable/) |
[Scikit-Image](http://scikit-image.org/) |

| What's in Third Party?
----|-----
Whether building from source or installing from the Python wheel, you also get complimentary tools installed as well. |
[Android cmake](https://github.com/taka-no-me/android-cmake) |
[benchmark](https://github.com/google/benchmark) |
[cnmem](https://github.com/NVIDIA/cnmem) |
[cub](http://nvlabs.github.io/cub/) |
[eigen](http://eigen.tuxfamily.org/) |
[googletest](https://github.com/google/googletest) |
[ios-cmake](https://github.com/cristeab/ios-cmake) |
[nccl](https://github.com/NVIDIA/nccl) |
[nervanagpu](https://github.com/NervanaSystems/nervanagpu) |
[NNPACK](https://github.com/Maratyszcza/NNPACK) |
[Google Protocol Buffers (protobuf)](https://developers.google.com/protocol-buffers/) |
[pybind11](https://github.com/pybind/pybind11) |