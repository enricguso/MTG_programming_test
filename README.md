#  Programming Test for the MTG researcher position

This repository contains the PyTorch (1.8+) implementation of the programming assignment for the researcher technical interview at the MTG. Contains the followings tasks:

1. Download the GTZAN dataset of music audio with genre annotations. 
2. Download Essentia’s MSD-MusiCNN TensorFlow model and extract deep embedding features for each track in the dataset.
3. Subtask 1. Evaluate music similarity based on these features (embeddings). Each song in the dataset has a single ground-truth genre label. Use these genres as a proxy for evaluating similarity, that is, consider two songs are similar when they have the same genre label. Compute average precision@10, MAP@10, and MAP@50 across the entire dataset. Report these results.
4. Subtask 2. Train a new transfer learning classifier using this dataset. Use the extracted audio features (embeddings) as an input to train a shallow target classifier. Report accuracy of the resulting model.

__Related Projects:__ [essentia-tensorflow](https://https://essentia.upf.edu/) |

### Visualizing the experiments from github.com
Simply open ```PROGRAMMING TEST.ipynb```.
### Installation

For installation we recommend to create a virtual environment as follows:
```
python -m venv <venv_name>
```
Then activate it:
```
source <venv_name>/bin/activate
```
And install dependencies:
```
pip install -r requirements.txt
```
Finally add the kernel to the jupyter lab:
```
python -m ipykernel install --user --name=<venv_name>
```
### Replicating the experiments
Run:
```
jupyter notebook
```
Open the ```PROGRAMMING TEST.ipynb``` file,  click "Kernel" tab and "Change Kernel". Select "<venv_name>" as kernel. For this GPU-essentia-tensorflow version, we recommend installing or downgrading to CUDA10.0.
