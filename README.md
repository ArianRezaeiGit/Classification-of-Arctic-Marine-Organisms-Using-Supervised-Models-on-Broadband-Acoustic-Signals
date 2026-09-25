# Classification of Arctic Marine Organisms Using Broadband Acoustic Signals

Python notebooks for classifying Arctic marine organisms from broadband acoustic spectra using supervised machine learning.

Models are trained on labelled mesocosm data at 120 and 200 kHz and applied to field observations from Nares Strait and the Beaufort Sea.

## Organisms

- **120 kHz:** Atlantic cod, polar cod, and shrimp.
- **200 kHz:** Atlantic cod, polar cod, shrimp, krill, and zooplankton.

## Notebooks

- **Classification modelling.ipynb** — Data preparation, model comparison, hyperparameter tuning, and evaluation.
- **Nares strait.ipynb** — Classification and temporal summaries of Nares Strait observations.
- **Beaufort Sea.ipynb** — Classification and summaries of Beaufort Sea observations.

The modelling workflow compares unnormalized and L2-normalized spectra and includes nested cross-validation for LightGBM and CatBoost. Field applications use LightGBM, with uncertain predictions labelled as **Unknown**.

## Running the code

The notebooks use Python, Jupyter, NumPy, pandas, Matplotlib, scikit-learn, LightGBM, CatBoost, Optuna, and joblib.

Input data and trained model files are not included. Update the file paths in each notebook before running. Saved outputs are available to view without rerunning the analyses.

## Author

Arian Rezaei
