# Python-Ubuntu-Venv-Setup

## Basics
python3 already installed on ubuntu.
        sudo apt install python3-pip, python3.8-venv
 
## Create Virtual Environment
        python -m venv venv
        source venv/bin/activate
from now `pip install` only installs packages inside the environment.
deactivate the environment with `deactivate`

## Source Control
Use `pip freeze > requirements.txt` to create something like a package.json file
Folder Structure:
        
        project
        |- venv
        |- requrements.txt
        |- src
Only include requirements.txt to source control, not the whole venv folder
To create the venv folder only based on requirements.txt file do:
        
        pip install -r requirements.txt
