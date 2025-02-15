# ChildSafetyProject
Age Detection and Age Group Classification using Touchscreen Gestures with Machine Learning

## Dataset
This project includes the Child_Safety_Data dataset (~5GB). It is located in the `Dataset` directory in a multi-part zip. To extract it, extract `Child_Safety_Data.zip` with 7-Zip on Windows or The Unarchiver on MacOS.

## Prerequisites
The notebooks in this project require **Python 3.11 or older**. We recommend using `pyenv` to manage multiple python versions and `venv` to create a virtual python environment specifically for this project. 

## Getting Start
* Clone this project with `git clone https://github.com/tbirms/ChildSafetyProject.git`
* Make a Python virtual environment with `python -m venv myenv`
* Activate the virtual environment with `souce myenv/bin/activate`
* Install requirements with `pip install -r requirements.txt`
If you are using a machine with lots of RAM (32GB>), we recommend running notebooks locally. If more RAM is required, we suggest using Google Colab to utilize one of their High-RAM runtime environments.

## Run Notebooks Locally in Visual Studio Code (Suggested)
* Install the Jupyter Extension for VS Code: https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter
* With the project open in VS Code, open any notebook in `Notebooks`
* Select the `myenv (Python)` kernel and start using the notebook

## Run Notebooks in Google Colab
* Open Google Drive and create a new directory `ChildSafetyProject`
* Unzip `Child_Safety_Data.zip` and upload the extracted dataset to this folder in Google Drive
* Open any notebook from `Notebooks` in Google Colab
* Connect to a High-RAM Runtime and start using the notebook
* Link Google Colab to Google Drive to access the dataset and create/restore Checkpoints

## Run Notebooks in Google Colab and connect to local runtime
* Open a new terminal and run command `python -m notebook --NotebookApp.allow_origin='https://colab.research.google.com' --port=8888 --NotebookApp.port_retries=0`
* Copy the token in the console to clipboard
* With a notebook open in Google Colab, select the Connection options dropdown and select "Connect to a local runtime"
* Paste the token at the end of the URL string and click Connect
* (Optional) You may provide your own token in the above command with option `--NotebookApp.token='c8de56fa4deed24899803e93c227592aef6538f93025fe01'` You MUST make this token unique!
