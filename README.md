# anaMamiTools

[![python](https://img.shields.io/badge/python->=3-blue.svg)](https://www.python.org/) [![anaconda](https://img.shields.io/badge/anaconda-3-blue.svg)](https://www.anaconda.com/)

This is **anaMamiTools**, a set of a Python- and Jupyter-based data handling and analysis tools for the STORM (former ELIOT) team experimental studies performed at the MAMI (MAinzer MIkrotron) B beamtest facility and focused on the electromagnetic interactions between high-energy particles and oriented crystalline lattices. In particular, measurements are taken of both the electromagnetic radiation emitted in the particle-crystal interaction, from the standpoint of the energy spectra &mdash; with a NaI+PMT detector, and the output beam 2D tansverse profile &mdash; with a LYSO screen placed across the beam path and framed by pixel cameras. Further information on both the particle-crystal interaction physics and on the experimental setup features can be found, for example, [here](http://cds.cern.ch/record/2626151).

In practice:
- **anaMamiDefl**(ection) performs the output beam spatial analysis, with the main focus on the case of channeling in bent cystalline targets; beam profile data are stored in TIFF files coming from the pixel cameras. It is optimised for the analysis of a dataset obtained with a single sample.
- **anaMamiRad**(iation) performs the analysis of the radiation data, which come from the NaI+PMT detector acquisition system and are stored in CNF (Canberra Nuclear File) files. It supports comparison between different-sample datasets.
- In order to easily handle the radiation data, it is necessary to convert the CNF files into formatted text files (TXT):  **cnfconv** by messlinger (on GitHub [here](https://github.com/messlinger/cnfconv)) was included in this bundle to ease this stage.

An extensive description of how these tools work can be found in the code comments.

Basic dependencies:

[![jupyterlab](https://img.shields.io/badge/jupyterlab-2-blue.svg)](https://jupyterlab.readthedocs.io/en/stable/) [![matplotlib](https://img.shields.io/badge/matplotlib-3.3.1-blue.svg)](https://matplotlib.org/) [![numpy](https://img.shields.io/badge/numpy-grey.svg)](https://numpy.org/) [![pandas](https://img.shields.io/badge/pandas-grey.svg)](https://pandas.pydata.org/) [![pip](https://img.shields.io/badge/pip-grey.svg)](https://pip.pypa.io/en/stable/) [![pyqt](https://img.shields.io/badge/pyqt-grey.svg)](https://riverbankcomputing.com/software/pyqt/intro) [![skimage](https://img.shields.io/badge/skimage-grey.svg)](https://scikit-image.org/) [![scipy](https://img.shields.io/badge/scipy-grey.svg)](https://www.scipy.org/)  [![succolib](https://img.shields.io/badge/succolib-grey.svg)](https://github.com/mattiasoldani/succolib) [![tqdm](https://img.shields.io/badge/tqdm-grey.svg)](https://github.com/tqdm/tqdm)

All these are automatically installed if using [Anaconda](https://www.anaconda.com/) (this project was developed and tested with Anaconda 3) and generating the environment described in the environment.yml file. In order to fully exploit the potential of these software tools, it is best to enable the interactive plots in the working environment. A Bash script is available to perform the complete installation of the environment itself, of the interactive mode and of other minor features; it could be run via
```shell
bash -i createEnvComplete.sh
```
Note: running the script via `./createEnvComplete.sh` won't work since the Bash interactive mode is needed.

The anaMamiTools set can be downloaded either as a ZIP archive, from the Code drop-down menu [here](https://github.com/mattiasoldani/anaMamiTools), or directly from the terminal (open in your project working directory) via
```shell
git clone https://github.com/mattiasoldani/anaMamiTools.git
```
Note: the latter requires  [Git](https://git-scm.com/) installed on your machine.

Found a bug? Or simply have any questions, comments or suggestions you'd like to talk about? Feel free to contact me at <mattiasoldani93@gmail.com>. And brace yourself, for the best is yet to come!
