# EM-DAT Python Tutorials

- [EM-DAT Python Tutorial 1: Basic Operations and Plotting](./python_tutorial_1_basic_operations_and_plotting.ipynb)
- [EM-DAT Python Tutorial 2: Making Maps](./python_tutorial_2_making_maps.ipynb).

**Note:** The Tutorials are also available on the [EM-DAT Documentation Website](https://doc.emdat.be/docs/additional-resources-and-tutorials/)

## Setting up

Windows (using conda in Anaconda Powershell prompt):

```powershell
cd <project directory>

# installing environment with conda
conda env create --name emdat -f environment.yml
conda activate emdat
# emdat env activated

# starting notebook server
jupyter notebook

# to leave emdat env
conda deactivate

# delete environment
conda env remove --name emdat
```

MacOS X and Linux (implying python=python3):

```bash
python -m venv myenv
source myenv/bin/activate
# myenv activated

pip install --upgrade pip
pip install -r requirements.txt
jupyter notebook

# to leave myenv
deactivate

# to delete local environment
rm -rf myenv
```