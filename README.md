# GraphTSNE
April 16, 2019
<br>

### Description
PyTorch implementation of the ICLR'19 paper:<br>
GraphTSNE: A Visualization Technique for Graph-Structured Data <br>
<br>
International Conference on Learning Representations 2019 <br>
Workshop for Representation Learning on Graphs and Manifolds <br>
ArXiv: https://arxiv.org/abs/1904.06915 <br>
Blog post: https://leowyy.github.io/graphtsne <br>

<p align="center">
   <img src="pic/graphtsne.gif" width="600"> <br>
   <b>GraphTSNE on the Cora Citation Network</b>
</p>

### Codes
The code `demo_notebook.ipynb` creates a visualization of the Cora citation network using GraphTSNE. The original Cora dataset and other citation networks can be found here: http://linqs.cs.umd.edu/projects/projects/lbc/.

The notebook takes roughly 3 minutes to run with GPU, or 8 minutes with CPU.
<br>

### Installation
   ```sh
   # Conda installation
   curl -o ~/miniconda.sh -O https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh # Linux
   curl -o ~/miniconda.sh -O https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh # OSX
   chmod +x ~/miniconda.sh
   ./miniconda.sh
   source ~/.bashrc

   # Clone GitHub repo
   git clone https://github.com/leowyy/GraphTSNE.git
   cd GraphTSNE

   # Install python libraries
   conda env create -f environment.yml
   conda activate graph_tsne
   python -m ipykernel install --user --name graph_tsne --display-name "graph_tsne"

   # Run the notebook
   jupyter notebook
   ```
   
### When should I use this algorithm?
For visualizing graph-structured data such as social networks, functional brain networks and gene-regulatory networks. Concretely, graph-structured datasets contain two sources of information: graph connectivity between nodes and node features.
<br>
