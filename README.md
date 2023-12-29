# Ex02 Django ORM Web Application
## Date: 10.11.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## ALGORITHM 

1.Clone the problem from GitHub


2.Create a new app in Django project


3.Enter the code for admin.py and models.py


4.Execute Django admin and create 10 Football players

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import foodball_player,foodball_playerAdmin
admin.site.register(foodball_player,foodball_playerAdmin)

models.py


from django.db import models
from django.contrib import admin
class foodball_player (models.Model):
    p_name=models.CharField(max_length=20)
    p_country=models.CharField(max_length=100)
    p_age=models.IntegerField()
    P_salary=models.IntegerField()
    p_email=models.EmailField()

class foodball_playerAdmin(admin.ModelAdmin):
   list_display=('p_name','p_country','P_salary','p_age','p_email')

```
## OUTPUT
![Alt text](<Screenshot (5).png>)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
