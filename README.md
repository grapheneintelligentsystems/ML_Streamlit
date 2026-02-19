## ML_Streamlit prototype with streamlit docker
ML tutorial

# requirements
python conda
streamlit
docker

# create a new enviroment in conda
'''
conda create --name streamlit
'''

# install requirements
streamlit
reportlab
scikit-learn
pandas
matplotlib
seaborn

# in a new command prompt activate conda envirment and install requirements automaticaly

```

pip install -r requirements.txt

conda env create --file environment.yml
conda install --yes --file requirements.txt
```
To generate the requirments automaticaly for the working enviroment do:

```
pip freeze > requirements.txt

```

then setup gitCLI to read or setup (name and email)

```

git config --global user.name

git config --global user.name "nameins"

git config --global user.email

git config --global user.name "nameins@...."

```

then add all files in git and push (see: https://www.atlassian.com/git/tutorials/saving-changes/git-commit)
```
git init  ##For first time only

git add .
git status
git commit -m "commit message"
git status
git push origin main

```

## Build local and Run local the Docker Image Using the Dockerfile
```sh
docker build -t streamlit-ml-app:latest .
```
```sh
docker run -p 8501:8501 streamlit-ml-app:latest
```

## On your browser
```sh
http://localhost:8501
```
