mkdir simple_app

create environment

```bash
conda create -n wineq python=3.7 -y
```

activate the environment

```bash
conda activate wineq
```

create a requirements.txt file

```bash
touch requirements.txt
```

install dependencies by adding below dependencies
==>dvc
==>dvc[gdrive]
==>scikit-learn

```bash
pip install -r requirements.txt 
```

touch README.md

touch template.py

download the data from
https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing


git init

dvc init

dvc add data_given/winequality.csv

git add . && git commit -m "first commit" 

create a new github repo
```bash
git branch -M main
git remote add origin https://github.com/shashiKumar14/simple-dvc-demo.git
```

git push -u origin main






















