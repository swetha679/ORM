# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a movie database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in the Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
admin.py

from django.contrib import admin
from.models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)

models.py


from django.db import models
from django.contrib import admin
class Movie (models.Model):
    mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField(max_length=10.0)


class MovieAdmin(admin.ModelAdmin):
    list_display=('mid', 'mname', 'collection', 'year', 'rating')



## OUTPUT


![Screenshot 2025-04-30 134844](https://github.com/user-attachments/assets/d2d01711-5abf-4a54-ade1-018d5901213a)


![Screenshot 2025-04-30 134905](https://github.com/user-attachments/assets/a6680b2d-e3fa-419d-b065-53a4fef9d327)



## RESULT
Thus, the program for creating a movie database using ORM has been executed successfully
