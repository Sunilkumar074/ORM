# Ex02 Django ORM Web Application
## Date: 22-03-2024
## Name: Sunil Kumar P.B
## Reg.no: 212223040213
## Dept: CSE

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-03-22 154650](https://github.com/Sunilkumar074/ORM/assets/152241049/8b0940de-4992-4fb6-ba7e-21466f1c12b7)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```
## OUTPUT

![Screenshot 2024-03-22 154511](https://github.com/Sunilkumar074/ORM/assets/152241049/41c97810-c94a-4f7b-a3b3-5dba819c1ec1)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
