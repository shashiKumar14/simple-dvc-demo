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

```bash
touch README.md
```

```bash
touch template.py
```


download the data from
https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing


```bash
git init
```

```bash
dvc init
```

```bash
dvc add data_given/winequality.csv
```

```bash
git add . && git commit -m "first commit" 
```

create a new github repo
```bash
git branch -M main
git remote add origin https://github.com/shashiKumar14/simple-dvc-demo.git
```
```bash
git push -u origin main
```

================================================================

# coding part

1)In params.yaml file add the input parameters and the output parameters and input/output paths

2)Create get_data.py in src folder . It reads params from param.yaml file & process and returns the dataframe

3)


















