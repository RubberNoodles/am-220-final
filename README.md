# Global Context for DiffDock Diffusion Confidence Model

In order to run this code, install the `requirements.txt`

```
python -m venv env
source env/bin/activate
pip install -r requirements.txt
```

Data was git-ignored, but is necessary to run the repo. Data must be extracted from PDBBind, with DiffDock inference to compute poses.

We also need DiffDock and esm.

```
git clone https://github.com/gcorso/DiffDock.git
cd DiffDock
git clone https://github.com/facebookresearch/esm.git
cd esm
pip install -e .
```
In order to the adjustments that I made to the code, you can either replace the files directly or run

```
cp score_model.py DiffDock/models/score_model.py
cp training.py DiffDock/utils/training.py
```

From here, we have all the necessary requirements to run the notebook.

