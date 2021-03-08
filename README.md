#  Programming Test for the MTG researcher position

This repository contains the PyTorch (1.2+) implementation of our branch of [Open-Unmix](https://github.com/sigsep/open-unmix-pytorch): a study on different loss functions for Music Source Separation.  For mor details on the architecture, visit the [main respository](https://github.com/sigsep/open-unmix-pytorch).

__Related Projects:__ [open-unmix-pytorch](https://github.com/sigsep/open-unmix-pytorch) | [musdb](https://github.com/sigsep/sigsep-mus-db) | [museval](https://github.com/sigsep/sigsep-mus-eval) | [norbert](https://github.com/sigsep/norbert)
### Visualizing the experiments

### Installation

For installation we recommend to use the [Anaconda](https://anaconda.org/) python distribution. To create a conda environment for _open-unmix_, simply run:
```
 conda install -c pytorch torchaudio 
```
```
pip install museval
```

`conda env create -f environment-X.yml` where `X` is either [`cpu-linux`, `gpu-linux-cuda10`, `cpu-osx`], depending on your system. For now, we haven't tested windows support.

### Replicating the experiments
Once installed, update the dataset and outpupt paths on `run_experiments.sh` and run it:
```bash
sh run_experiments.sh
```

