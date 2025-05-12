All notebooks assume you have successfully installed the CMB-ML package.

Instructions are rough currently as we rearrange things. Please contact us if you have issues.

# Installation

- The base CMB-ML content is needed. Follow the instructions in the [main repository](https://github.com/CMB-ML/cmb-ml.git).
- Activate the conda environment
    - `conda activate cmb-ml`
- Clone this repository
    - `git clone https://github.com/CMB-ML/cmb-ml-tutorials.git`
- Update the environment
    - `cd <whatever>` (Where `whatever` contains this `README.md` and the `env.yaml`)
    - `conda env update -n cmb-ml -f env.yaml`

Now you should be set up to use these notebooks.

# Demonstrations

CMB-ML manages a complex pipeline that processes data across multiple stages. Each stage produces outputs that need to be tracked, reused, and processed in later stages. Without a clear framework, this can lead to disorganized code, redundant logic, and errors.

The CMB-ML library provides a set of tools to manage the pipeline in a modular and scalable way. 

We include a set of demonstrations to help with both installation and introduction to core concepts. The first introduces our approach configuration management. That background paves the way to set up a local configuration and get the required files. Following this are a series of tutorials for the Python objects.

Most of these are in jupyter notebooks:
- [Hydra and its use in CMB-ML](./demonstrations/A_hydra_tutorial.ipynb)
- [Hydra in scripts](./demonstrations/B_hydra_script_tutorial.ipynb) (*.py files)
- [Setting up your environment](./demonstrations/C_setting_up_local.ipynb)
- [Getting and looking at simulation instances](./demonstrations/D_getting_dataset_instances.ipynb)
- [CMB_ML framework: stage code](./demonstrations/E_CMB_ML_framework.ipynb)
- [CMB_ML framework: pipeline code](./demonstrations/F_CMB_ML_pipeline.ipynb)
- [CMB_ML framework: Executors](./demonstrations/G_CMB_ML_executors.ipynb)

Only the Setting up your environment is really critical, though the others should help.

I'm interested in hearing what other demonstrations would be helpful. Please let me know what would be helpful. I've considered these notebooks:
- Executors, continued: showing how executors are set up for PyTorch training/inference and matplotlib figure production
- Looking at actual pipeline stages and explaining them
- Paper figure production (available, in another repository, need cleaning)
