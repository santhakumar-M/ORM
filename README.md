# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
clone the repository to the idea. start a new inside the project folder

### STEP 2:
type the appropriate code for your table and provide appropriate data types to the columns

### STEP 3:
create a report about projects in readme.md file and upload the django_orm_app folder to your remote repository

## PROGRAM
```python
from django.db import models
from django.contrib import admin
# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```
## OUTPUT
![san](https://user-images.githubusercontent.com/121998012/230138169-9175fee7-709c-4db5-b1fb-ff94fe7b8f95.jpg)

## RESULT
Thus the project is developed to have student information database.
