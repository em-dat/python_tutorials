# EM-DAT Python Tutorials

- [EM-DAT Python Tutorial 1: Basic Operations and Plotting](./python_tutorial_1_basic_operations_and_plotting.ipynb)
- [EM-DAT Python Tutorial 2: Making Maps](./python_tutorial_2_making_maps.ipynb)
- [EM-DAT Python Tutorial 3: Augmenting EM-DAT Data with AI Agents and Web Search](./python_tutorial_3_augmenting_data_with_ai_agents.ipynb)

**Note:** The Tutorials are also available on the [EM-DAT Documentation Website](https://doc.emdat.be/docs/additional-resources-and-tutorials/)

## Setting up

We recommend [uv](https://docs.astral.sh/uv/), which installs Python and the packages listed in `pyproject.toml`, at the versions locked in `uv.lock`. After [installing uv](https://docs.astral.sh/uv/getting-started/installation/), run from the project directory:

```bash
# create the .venv environment and install the packages
uv sync

# start the notebook server
uv run jupyter notebook
```

To delete the environment, delete the `.venv` folder.

Tutorial 3 also needs a Mistral API key in the `MISTRAL_API_KEY` environment variable. You can write it in a `.env` file, which git ignores, as `MISTRAL_API_KEY=your-key`, and start the server with:

```bash
uv run --env-file .env jupyter notebook
```

Variables already set on your system take precedence over the file.

### Alternative: pip

With Python 3.11 or later, `requirements.txt` lists the same package versions:

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

With conda, create and activate an environment with Python 3.11 or later, then run the `pip install` command.
