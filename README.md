# Ex02 Django ORM Web Application
## Name: sugeshan
## Reg.no: 212224040337
## Date: 03.04.2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ER Diagram

![Entity rel pic](https://github.com/user-attachments/assets/0bce9687-4d45-46aa-8e47-b3fab138bad5)


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

admin.py
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

```
models.py
```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```

## OUTPUT

![output](https://github.com/user-attachments/assets/da4de25c-9fc4-4d7e-b76f-301d70c8275c)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
