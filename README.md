All notebooks assume you have successfully installed the CMB-ML package.

Instructions are rough currently as we rearrange things. Please contact us if you have issues.

# Installation of CMB-ML framework

- Download the CMB-ML repository
    - `git clone git@github.com:CMB-ML/cmb-ml.git`
    - `cd cmb-ml`
    - `git switch whatever`
- Create the conda environment 
    - remove old conda installations (and Poetry... which can be gotten rid of as a whole)
        - `conda remove -n cmb-ml --all`
    - still required due to either namaster or torch... this could be fixed soon, possibly
    - `conda env create -f env.yaml`
    - To change the name of the environment, edit the file or use a different command.
- Activate the conda environment
    - `conda activate cmb-ml`
- Install CMB-ML
    - `which pip` (ensure that the response is within the conda environment)
    - `pip install .`
- Update the environment
    - `cd <whatever>` (Where `whatever` contains this `README.md` and the `env.yaml`)
    - `conda env update -n cmb-ml -f env.yaml`

Now you should be set up to use these notebooks.