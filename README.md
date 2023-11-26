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

3)Create load_data.py in src folder . It gets the data from get_data.py in src folder . using the functions it calls and stores the csv into data/raw folder.

4)In dvc.yaml file add the first stage.It has cmd,input dependencies,output paths

5)dvc repro

6)Create split_data.py in src folder . It reads params from param.yaml file then takes the data from raw folder and splits it into train and test and then inserts it into processed folder.

7)continue 4th and 5th step

8)create train_and_evaluate.py in src folder . It reads params from param.yaml file and takes the data from processed folder and it trains and evaluates the data 

9)continue 4th and 5th step

10)install necessary dependencies if any like tox,pytest

11)create tox.ini file e.x: touch tox.ini

12)create tests folder and create inside __init__.py,conftest.py,test_config.py 

13)To run the test cases command is : pytest -v .
==>inthis code writing the test cases in test_config.py .For the functions have to use  prefixed with "test_" 

14)





















