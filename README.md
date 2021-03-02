# install


## install numpy in macOS Apple Silicone M1

1. install and activate environment
```shell
python3 -m venv venv
source venv/bin/activate
```
2. install Cython
```shell
pip3 install Cython
```
3. checkout version of numpy from source code
```shell
mkdir numpy
git clone https://github.com/numpy/numpy.git
cd numpy
git checkout v1.20.1
```
4. build and install
```shell
pip3 install . --no-binary :all: --no-use-pep517
```
5. cleanup
```shell
cd ../
rm -rf numpy
```
