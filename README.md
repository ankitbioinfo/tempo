# NiCo: Niche Covariation Analysis 

Developed by Ankit Agrawal (c) Grün lab 2024

NiCo package designed to uncover covariation patterns between interacting cell types from image-based single-cell resolution spatial transcriptomics data. It enables comprehensive cell type annotations, niche interaction discoveries, and the analysis of covariation patterns between interacting cell types.


### Key Features <br> 
Cell Type Annotation: Perform accurate cell type annotations on spatial transcriptomics data. <br> 
Niche Interaction Analysis: Identify and analyze interactions between different cell types within their tissue niches. <br> 
Covariation between colocalized cell types: Discover covariation patterns between interacting cell types to understand their covariate <br>.

Find covariation patterns between interacting cell types from image-based single cell resolution spatial transcriptomics data.


A package that performs cell type annotations on spatial transcriptomics data, finds the niche interactions and covariation patterns between interacting cell types.

Ready for use! Tutorials and Documentation are available!


## Install the NiCo package using the conda environment.  

```shell
conda create -n nicoUser python=3.11
conda activate nicoUser
pip install nico-sc-sp
pip install jupyterlab
```

Sometimes, the pygraphviz package cannot be installed via pip, or during the cell type interaction part it gives error that "neato" not found in path so an alternative conda way of installation is recommended. Please follow the installation of pygraphviz [here](https://pygraphviz.github.io/documentation/stable/install.html)

```console
conda create -y -n nicoUser python=3.11
conda activate nicoUser
conda install -c conda-forge pygraphviz
pip install nico-sc-sp
pip install jupyterlab
```

# Required packages built upon
By default, these packages should install automatically.
But if any version conflict exists, the user can install the specific version independently using pip command.
```shell
scanpy==1.9.6
seaborn==0.12.2
scipy==1.11.3
matplotlib==3.7.3
numpy==1.26.1
gseapy==1.0.6
xlsxwriter==3.1.9
numba==0.58.1
pydot==1.4.2
KDEpy==1.1.8
pygraphviz==1.11
networkx==3.2.1
scikit-learn==1.3.2
pandas==2.1.1
leidenalg
```

# Import the functions from the Python prompt in the following way.  

```python
from nico import Annotations as sann
from nico import Interactions as sint
from nico import Covariations as scov
```



# Tutorials
Please follow the NiCo tutorial here. <br> 
https://github.com/ankitbioinfo/nico_tutorial 

# Documentations

Please follow the NiCo documentation here. <br>
https://nico-sc-sp.readthedocs.io/en/latest/

# Reference 
Ankit Agrawal, Stefan Thomann, Sukanya Basu, Dominic Grün. NiCo Identifies Extrinsic Drivers of Cell State Modulation by Niche Covariation Analysis. Submitted, 2024


# Check out more:
Thanks to the following two utils packages used to develop NiCo.

SCTransformPy <br>
https://github.com/atarashansky/SCTransformPy

pyliger <br> 
https://github.com/welch-lab/pyliger
