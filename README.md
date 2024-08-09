# Graph Neural Networks Demonstration
This repository includes a Jupyter Notebook to display and run a simple Graph Neural Network. 

## Requirements

To setup the software in this repository under an Anaconda environment follow:

```
conda create --gnndemo myenv python=3.9
```

Before you run `requirements.txt` be sure to run:

```
conda install rvlib
```

Then run

```
pip install -r requirements.txt
```

There are 2 additional steps:

- Install C++ build tools from Microsoft Visual Code
- Fix the import in the temporal GNN (due to `PyG > 2.5.0`)


To fix the import navigate to: `C:\Users\<YOUR USER>\anaconda3\envs\gnnenv2\Lib\site-packages\torch_geometric_temporal\nn\attention\tsagcn.py`

and then change `from torch_geometric.utils.to_dense_adj import to_dense_adj` to `from torch_geometric.utils import to_dense_adj`

## Usage

To run a Jupyter Notebook you can type, the following in any anaconda prompt shell:

```
jupyter lab
```

An alternative could be [VS Code](https://code.visualstudio.com/)
