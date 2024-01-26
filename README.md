# Face Similarity API

## Introduction

Welcome to the Face Similarity API project! The Face Similarity API is designed to measure the similarity between a facial photo (e.g., ID card, driver's license, passport) and an input photo. This API provides a convenient way to assess the likeness of faces and is useful for various applications, including identity verification and facial recognition.

## Features

The Face Similarity API offers the following key features:

- **Face Comparison**: Compare a reference facial photo (e.g., an official ID) with an input facial photo to determine the degree of similarity.
- **Scalable**: The API can handle a wide range of input images and is suitable for both small-scale and large-scale applications.
- **Accurate**: Utilizes advanced facial recognition algorithms to provide accurate similarity scores.


### Step  to use

Here step to use the project, this project use django as frame work

#### Open a Terminal/Command Prompt and Follow the Steps Below


Create a virtual environment using the following command:


```
python -m venv venv
```

Activate the created virtual environment:


```
.\venv\Scripts\activate
```

Upgrade Pip


Ensure that your Pip is up to date. You can check your Pip version using the following command:

```
python -m pip install --upgrade pip
```

Install the requirements from requirements.txt:

``` 
pip install -r requirements.txt
```

Lalu pindah ke directory project
```
cd .\image_project\
```
Perform migrations to create database tables. To create migrations, use the following command:

```
python manage.py makemigrations
``` 
After creating migrations, apply them to the database using the following command:

```
python manage.py migrate --run-syncdb
```

Once the migrations are applied, you can run the Django server. To start the Django server, use the following command:

```
python manage.py runserver
```

To input the first image:
```
http://127.0.0.1:8000/fsim/upload-anchor/
```

To Predist similarity:
```
http://127.0.0.1:8000/fsim/predict-similarity/
```