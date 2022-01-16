# EasyModerationKit

EasyModerationKit is a public transparency statement. It declares any repositories and legalities used in the EasyModeration system. It allows for implementing EasyModeration into an advanced character/word/phrase detection system.

## Installation

EasyModerationKit Dependencies

  * [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)
  * [TensorFlowTTS](https://github.com/TensorSpeech/TensorFlowTTS)
  * [scikit-fuzzy](https://github.com/scikit-fuzzy/scikit-fuzzy)
  * [Detoxify](https://github.com/unitaryai/detoxify)
### PaddleOCR

1. Install PaddleOCR Whl Package

```bash
pip install "paddleocr>=2.0.1" # Recommend to use version 2.0.1+
```

- **For windows users:** If you getting this error `OSError: [WinError 126] The specified module could not be found` when you install shapely on windows. Please try to download Shapely whl file [here](http://www.lfd.uci.edu/~gohlke/pythonlibs/#shapely).

  Reference: [Solve shapely installation on windows](https://stackoverflow.com/questions/44398265/install-shapely-oserror-winerror-126-the-specified-module-could-not-be-found)

- **For layout analysis users**, run the following command to install **Layout-Parser**

  ```bash
  pip3 install -U https://paddleocr.bj.bcebos.com/whl/layoutparser-0.0.0-py3-none-any.whl
  ```

<a name="2-easy-to-use"></a>

### TensorFlowTTS
Installation with pip
```bash
$ pip install TensorFlowTTS
```
### scikit-fuzzy
Installation

Scikit-Fuzzy depends on

  * NumPy >= 1.6
  * SciPy >= 0.9
  * NetworkX >= 1.9

and is available on PyPi! The latest stable release can always be obtained
and installed simply by running

    $ pip install -U scikit-fuzzy

which will also work to upgrade existing installations to the latest release.


If you prefer to install from source or develop this package, you can fork and
clone this repository then install SciKit-Fuzzy by running

	$ python setup.py install

or develop locally by running

	$ python setup.py develop

If you prefer, you can use SciKit-Fuzzy without installing by simply exporting
this path to your PYTHONPATH variable.

### Detoxify
How to run   

First, install dependencies   
```bash
# clone project   

git clone https://github.com/unitaryai/detoxify

# create virtual env

python3 -m venv toxic-env
source toxic-env/bin/activate

# install project   

pip install -e detoxify
cd detoxify

# for training
pip install -r requirements.txt

```   
## License
Read [LICENSE.txt](/LICENSE) for more information.
