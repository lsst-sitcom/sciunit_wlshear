# sciunit_wlshear
Analysis notebooks and demos relevant to WL Shear Science Unit.

These are primarily intended to be run at the Rubin Science Platform and S3DF.


To automate this, install the pre-commit hook.
This is a one-time setup.

From a terminal at S3DF
```bash
pre-commit install
```

`pre-commit` command will be availabe from terminal once you have setup the shared stack following the steps below.

## How to setup this repository
This is a one-time setup.

1. Login to the [Rubin Science Platform](https://usdf-rsp.slac.stanford.edu/)
2. Under your workspace, clone this repo
```bash
git clone https://github.com/lsst-sitcom/sciunit_wlshear.git
```
3. Open a Terminal, e.g., from File > New > Terminal
4. Follow the instruction to setup the stack. It should be
```bash
source /opt/lsst/software/stack/loadLSST.sh
setup lsst_sitcom
```
5. Setup pre-commit
```bash
pre-commit install
```

## How to work on this repository
Cloning this repo instead of creating multiple copies helps to keep all notebooks consolidated and synchronized.
Please feel free to contribute your own notebooks to this repository.

1. Login to the [Rubin Science Platform](https://usdf-rsp.slac.stanford.edu/)
2. For DP2 specific analysis, navigate to the `sciunit_wlshear/notebooks/dp2` directory.
3. Create a branch to work on extending or creating new notebooks
```bash
git checkout -b u/<github-id>/<your-branch-name>
```
There is no particular rule about naming, but having this structure avoids clashes.
4. When you have some results to share, please commit and push your changes to GitHub.
```bash
git add <list-of-changed-files-separated-by-whitespace>
git commit -m "Your commit message"
git push
```

### Important Note

Since the data at S3DF, particularly images, are not public yet, it is important to clear any notebook outputs before pushing to this repository.
Because it is easy to miss, please install the pre-commit hook to automate this process using the setup instructions above.
