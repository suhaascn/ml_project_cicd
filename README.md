# ml_project_cicd
This is the first CI/CD  machine learning project 

Application url: HousingPredictor

## Start Machine Learning project.

### Software and account Requirement.

1. [Github Account](https://github.com/)
2. [Heroku Account](https://id.heroku.com/login)
3. [VS Code IDE](https://code.visualstudio.com/download)
4. [GIT cli](https://git-scm.com/downloads)
5. [GIT Documentation](https://git-scm.com/docs/gittutorial)


Creating conda environment : As a standard pratice its created seprately for each project.
```
conda create -p venv python==3.7 -y              
conda activate venv/
```
venv is the name of the virtual enviornment
an we name the version intrested.
-p virtual env will be availble in project file 
-n usually create on conda

OR
```
conda activate venv
```
```
pip install -r requirements.txt
```

To Add files to git

```
git add .conda
```
OR
```
git add <file_name>
```

Note: To ignore file or folder from git we can write name of file/folder in .gitignore file

To check the git status
```
git status
```

To check all version maintained by git
```
git log
```

To create version/commit all changes by git
```
git commit -m "message"
```

To send version/changes to github
```
git push origin main
```
To check remote url
```
git remote -v
```

To setup CI/CD pipeline in heroku we need 3 information
HEROKU_EMAIL = anishyadav7045075175@gmail.com
HEROKU_API_KEY = <>
HEROKU_APP_NAME = ml-regression-app
BUILD DOCKER IMAGE

docker build -t <image_name>:<tagname> .
Note: Image name for docker must be lowercase

To list docker image

docker images
Run docker image

docker run -p 5000:5000 -e PORT=5000 f8c749e73678
To check running container in docker

docker ps
Tos stop docker conatiner

docker stop <container_id>
python setup.py install
Install ipykernel

pip install ipykernel
Data Drift: When your datset stats gets change we call it as data drift

Write a function to get training file path from artifact dir
