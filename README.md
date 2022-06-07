# CheckHate


CHECKHATE is an application that uses deep learning techniques to detect and classify harmful texts in Filipino language.

This project is developed by: 

* A. Aloveros (THW)
* C. Encinares (THW)
* J. Doros (THW)
* R. Delos Reyes (THW)

## Installation
You may opt to [activate a virtual environment](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/) before installing the dependencies.

1. Open the terminal
2. Change the directory to the project's root directory
3. Install the dependencies in `requirements.txt`:

```cmd
> pip install -r requirements.txt
```
4. You may encounter problems installing wordcloud. If that happens, follow these steps:

    - Download the .whl file compatible with your Python version and your windows distribution (32bit or 64bit) [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#wordcloud)
    - Change your directory to the path containing the downloaded .whl file
    - Run this command, replacing `<filename>` to the name of the .whl file previously downloaded (e.g. `wordcloud‑1.8.1‑cp310‑cp310‑win_amd64.whl`):
  
    ```cmd
    > python -m pip install <filename>
    ```
  
### Running the models

1. Open Jupyter Notebook
```cmd
> jupyter notebook
```

(Alternatively, if you are already using Visual Studio Code, you can directly follow Step 2 instead of opening Jupyter Notebook)

2. Go to "models"
3. Open your chosen python notebook:
    - `explanation.ipynb`: Template (basic) notebook used to explain the implementation of the models (Naive Bayes, LSTM)
    - `models_raw.ipynb`: Notebook used to implement the models using raw (unmodified/uncorrected) Filipino data
    - `models_clean.ipynb`: Notebook used to implement the models using clean (modified/corrected) Filipino data
    - `models_translated.ipynb`: Notebook used to implement the models using clean Google Translated English data
4. Click `Run All`. (If you are in Visual Studio Code and you initially opted to create a virtual environment, make sure that you have selected the correct kernel before running the model. The `Select Kernel` button is found on the top right of the VSCode window.)
