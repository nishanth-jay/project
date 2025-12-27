# Project Responsive Web Design using Bootstrap
# Date:15-12-2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
pro.html

{% load static %}
<html>
<head>
    <title>watch</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="{% static 'display.css' %}">
</head>
<body>

<nav class="navbar px-4 bg-light">
    <a class="navbar-brand fw-bold" href="#">STOCKS</a>

    <ul class="navbar-nav flex-row ms-4">
        <li class="nav-item me-3"><a class="nav-link" href="#">home</a></li>
        <li class="nav-item me-3"><a class="nav-link" href="#">collections</a></li>
        <li class="nav-item me-3"><a class="nav-link" href="#">order</a></li>
    </ul>
</nav>

<section class="text-center p-3 text-white">
    <h2>WONDER WATCHES</h2>
</section>

<div class="container my-4">
    <div class="row row-cols-6 g-4">

        <div class="col">
            <div class="card">
                <img src="{% static 'metallic.jpeg' %}">
                <div class="card-body">
                    <b>METALIC</b>
                    <p class="small">RS-1,699</p>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="card">
                <img src="{% static 'silver.webp' %}">
                <div class="card-body">
                    <b>SILVER</b>
                    <p class="small">RS-7,999</p>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="card">
                <img src="{% static 'matteblack.jpg' %}">
                <div class="card-body">
                    <b>MATTE-BLACK</b>
                    <p class="small">RS-1,699</p>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="card">
                <img src="{% static 'goldpolish.jpg' %}">
                <div class="card-body">
                    <b>GOLD POLISHED</b>
                    <p class="small">RS-9,999</p>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="card">
                <img src="{% static 'straps.jpg' %}">
                <div class="card-body">
                    <b>STRAPS</b>
                    <p class="small">RS-450</p>
                </div>
            </div>
        </div>

        <div class="col">
            <div class="card">
                <img src="{% static 'battery.jpg' %}">
                <div class="card-body">
                    <b>BATTERY</b>
                    <p class="small">RS-300</p>
                </div>
            </div>
        </div>

    </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
```
views.py

from django.shortcuts import render

def fun(request):
    return render(request, 'pro.html')
```
```
urls.py

from django.contrib import admin
from django.urls import path
from environment import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('',views.fun),
]
```
# OUTPUT:
![alt text](<Screenshot 2025-12-27 115757.png>)
# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
