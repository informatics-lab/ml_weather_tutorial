# Environments for ML Weather Tutorial
This directory contains files which define conda environments for use in the ML weather tutorial. There are two sets of files, conda requirements fles and conda lock files

## Install from requirements files
* conda equirements files - these provide a definiiton of the key packages to be installed, but don't specify the exact build or all packages. Conda will workout all the dependencies that need to be installed. The advantage is that this is more robust over time, but the disadvantage is that the dependency can take a long time and a lot of memory.

There are 2 requirements files definied:
* `requirements_sklearn.yml` - For  running notebooks 1,2,4
* `requirements_tensorflow.yml` - For  running notebook 3

You can create environment with the following commands, run from the local repo root:
```bash
conda env create --file environments/requirements_sklearn.yml
conda env create --file environments/requirements_tensorflow.yml
```

* ## Install from lock files
Conda lock files provide more definiition. These are strictly speaking not actual lock files, which rquires a separate library, but rather requirements files with all the buold info specified. The advantage is that there is no dependency resolution, so it is much quicker. The disadvantage is that  you won't get versions of lubraries with the latest bug fixes, and each file is specific to a platform, so it is not portable like the requirements files definied above.

There are "lock" files defined for the Met Office linux environment:
* `req_sklearn_spice_lock.yml` - For  running notebooks 1,2,4
* `req_tensorflow_spice_lock.yml` - For  running notebook 3

You can create environment with the following commands, run from the local repo root:
```bash
conda env create --file environments/req_sklearn_sklearn_lock.yml
conda env create --file environments/req_sklearn_tensorflow_lock.yml
```

For more info see [Setup wiki page](../../wiki/Setup-Instructions)
