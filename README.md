# Fragile

[![Travis build status](https://travis-ci.com/FragileTech/fragile.svg)](https://travis-ci.com/FragileTech/fragile)
[![Documentation Status](https://readthedocs.org/projects/fragile/badge/?version=latest)](https://fragile.readthedocs.io/en/latest/?badge=latest)
[![Code coverage](https://codecov.io/github/FragileTech/fragile/coverage.svg)](https://codecov.io/github/FragileTech/fragile)
[![PyPI package](https://badgen.net/pypi/v/fragile)](https://pypi.org/project/fragile/)
[![Latest docker image](https://badgen.net/docker/pulls/fragiletech/fragile)](https://hub.docker.com/r/fragiletech/fragile/tags)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
[![license: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![stable](https://badges.github.io/stability-badges/dist/stable.svg)](https://github.com/badges/stability-badges)

Fragile is a framework for developing optimization algorithms inspired by Fractal AI and running them at scale.

## 🔥 Features

- Provides classes and an API for easily developing planning algorithms
- Provides an classes and an API for function optimization
- Built-in visualizations of the sampling process
- Heavily documented and tested
- Support for parallelization and distributed search processes

## 🌀 FractalAI

FractalAI is based on the framework of [non-equilibrium thermodynamics](https://en.wikipedia.org/wiki/Non-equilibrium_thermodynamics), and can be used to derive new mathematical tools for efficiently exploring state spaces.

The principles of our work are accessible online:

- [Arxiv](https://arxiv.org/abs/1803.05049) manuscript describing the fundamental principles of our work.
- [Blog](http://entropicai.blogspot.com) that describes our early research process.
- [Youtube channel](https://www.youtube.com/user/finaysergio/videos) with videos showing how different prototypes work.
- [GitHub repository](https://github.com/FragileTech/FractalAI) containing a prototype that solves most Atari games.

## 📓 Examples

Check out the [getting started](https://fragile.readthedocs.io/en/latest/resources/examples/01_getting_started.html)
section of the docs, or the [examples](https://github.com/FragileTech/fragile/tree/master/examples) folder.

Try out select Fragile demos directly from Google Colab:

| Notebook                                                                                                     | Description                                                                                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`function_minimization`][function_minimization]<br />[![Open in Colab][colab]][function_minimization_colab] | There are many problems where we only need to sample a single point instead of a trajectory. The `optimize` module provides environments and models that help explore function landscapes in order to find points that meet a desired Min/Max condition. |

[colab]: https://colab.research.google.com/assets/colab-badge.svg
[function_minimization]: examples/02_function_minimization.ipynb
[function_minimization_colab]: https://colab.research.google.com/github/FragileTech/fragile/blob/master/examples/02_function_minimization.ipynb

## 🐳 Docker

Fragile publishes a [Docker container that launches a Jupyter notebook](https://hub.docker.com/r/fragiletech/fragile) accessible on port **8080** with password: `fragile`

You can pull the docker image from [Docker Hub](https://hub.docker.com/) by running:

```bash
docker pull fragiletech/fragile:version-tag
```

Where `version-tag` corresponds to the fragile version that will be installed in the pulled image.

## 💾 Installation

Intall Fragile with `pip`:

```bash
pip install fragile[all]
```

> Fragile has been tested on Ubuntu 18.04 with Python 3.6, 3.7 and 3.8. If you experience any problems running it on a different OS, [open an issue](https://github.com/FragileTech/fragile/issues/new).

Detailed installation instructions can be found in the [docs](https://fragile.readthedocs.io/en/latest/resources/installation.html).

## 📖 Documentation

You can access the documentation on [Read The Docs](https://fragile.readthedocs.io/en/latest/).

## 🗺 Roadmap

Upcoming features: _(not necessarily in order)_

- Add support for saving visualizations.
- Fix documentation and add examples for the `distributed` module
- Upload Montezuma solver
- Add new algorithms to sample different state spaces.
- Add a module to generate data for training deep learning models
- Add a benchmarking module
- Add deep learning API

## 👷‍♀️ Contributing

Contributions are welcome! Please take a look at [contributining](docsrc/markdown/CONTRIBUTING.md)
and respect the [code of conduct](docsrc/markdown/CODE_OF_CONDUCT.md).

## 📝 Cite us

If you use this framework in your research please cite us as:

    @misc{1803.05049,
        Author = {Sergio Hernández Cerezo and Guillem Duran Ballester},
        Title = {Fractal AI: A fragile theory of intelligence},
        Year = {2018},
        Eprint = {arXiv:1803.05049},
    }

## ⚖️ License

This project is MIT licensed. See `LICENSE.md` for the complete text.
