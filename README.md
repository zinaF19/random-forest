# Random Forest

A hands-on introduction to random forests for classification. You build a random forest with scikit-learn, see how it improves on a single decision tree, evaluate and tune it, and then apply the full workflow yourself to predict loan defaults on Lending Club data.

## Learning Objectives

By the end of this repository, you should be able to:

- Build and train a random forest classifier with scikit-learn.
- Describe how a random forest improves on a single decision tree.
- Prepare real-world data for tree-based models.
- Evaluate and tune a classification model.
- Interpret model results and feature importances.
- Apply the full workflow to a new prediction problem.

## Learning Path

Work through the notebooks in order:

| File / Folder | Description |
|---|---|
| [**1 - Random Forest Codealong**](1_random_forest_codealong.ipynb) | Implement a random forest with scikit-learn and read its predictions. |
| [**2 - Random Forest Tutorial**](2_random_forest_tutorial.ipynb) | Compare a decision tree with a random forest across a full workflow: clean the data, impute missing values, train a baseline, then tune with randomized search. |
| [**3 - Random Forest Exercise**](3_random_forest_exercise.ipynb) | Apply the workflow yourself on Lending Club loan data, building both a decision tree and a random forest. |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**Helper and Plotting Functions**](helper_and_plotting_functions.py) | Shared functions for evaluating models and plotting results. |
| [**Solutions**](solutions/) | Reference solutions. |
| [**data.zip**](data.zip) | The datasets, bundled as a zip (unzip it during setup). |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Dependency lock file. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a **placeholder**. Replace it including the `< >` brackets with your own value. For example, `cd <repo-name>` becomes `cd ds-random-forest`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in (`.venv/`).

```bash
cd <repo-name>
uv sync
```

---

### 5. Unzip the Data

The datasets are bundled in `data.zip`. Extract them into a `data/` folder before running the notebooks. This command uses the environment from `uv sync`:

```bash
uv run python -c "import zipfile; zipfile.ZipFile('data.zip').extractall()"
```

---

### 6. Open the Notebooks

> [!NOTE]
> Make sure you open VS Code from the project root so it automatically detects the environment created by `uv sync`.

Launch VS Code in the project root folder:

```bash
code .
```

Then open a notebook and select the Python environment created by `uv sync` as the kernel.

## References & Further Reading

- [**Scikit-learn: Ensemble methods**](https://scikit-learn.org/stable/modules/ensemble.html): How forests of randomized trees, bagging, and boosting work.
- [**Scikit-learn: RandomForestClassifier**](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html): The API reference for the classifier used here.
- [**Scikit-learn: Feature importances with a forest of trees**](https://scikit-learn.org/stable/auto_examples/ensemble/plot_forest_importances.html): Reading impurity-based and permutation feature importances from a random forest.
- [**Scikit-learn: Tuning hyperparameters**](https://scikit-learn.org/stable/modules/grid_search.html): Grid search, randomized search, and successive halving.
