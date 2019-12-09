# pydrobert

`pydrobert` is the namespace I use for the python utilities that I redistribute open source. Subpackage `XXX` can be found on PyPI with the name `pydrobert-XXX` and on Conda with the same name on the channel `sdrobert`:

``` bash
pip install pydrobert-XXX
conda install -c sdrobert pydrobert-XXX
pip install git+https://github.com/sdrobert/pydrobert-XXX  # bleeding edge
```

The package can then be imported via

``` python
import pydrobert.XXX
```

***This is student-driven code, so don't expect a stable API. I'll try to use semantic versioning, but the best way to keep functionality stable is by pinning the version in the requirements or by forking.***

## Available Packages

- [pydrobert-kaldi](https://github.com/sdrobert/pydrobert-kaldi): Pythonic bindings for Kaldi I/O. Unlike other packages,
  `pydrobert-kaldi` needs no external Kaldi installation to work. Compiled for Windows, OSX, and Linux.
- [pydrobert-param](https://github.com/sdrobert/pydrobert-param): Intuitive hyperparameter (de)serialization that couples with the
  `param` package. Includes hooks to read parameters in from a file automatically using `argparse` arguments.
- [pydrobert-pytorch](https://github.com/sdrobert/pydrobert-pytorch): PyTorch modules, utilities, and various bits-and-bobs I use
  when building models for PyTorch. Includes gradient estimators, edit-distance-based metrics, data loaders, experiment management,
  attention mechanisms, and other things.
- [pydrobert-speech](https://github.com/sdrobert/pydrobert-speech): Digital signal processing for speech. This includes the
  standard Mel-scaled filter banks, and so much more. The results can be saved to NumPy, PyTorch, or Kaldi.

## Defunct Packages

- [pydrobert-gpyopt](https://github.com/sdrobert/pydrobert-gpyopt): Wrappers to make GPyOpt more accessible. PyPI only. Dumped
  in favour of Optuna.

## Licensing

All subpackages are [Apache 2.0 licensed](https://tldrlegal.com/license/apache-license-2.0-%28apache-2.0%29).

## How To Cite

If you use any pydrobert subpackage in an academic publication, please cite as follows:

```
@misc{robertsonPydrobert2019,
	title = {pydrobert},
	url = {https://github.com/sdrobert/pydrobert},
	author = {Robertson, Sean},
	year = {2019}
}
```
