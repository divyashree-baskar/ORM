# Ex02 Django ORM Web Application
## Date: 09/04/2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/88eca29d-8f77-42a9-a09a-36d14eb58170)





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
class Employee(models.Model):
    eid = models.CharField(max_length=20, help_text="Employee ID")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display = ('eid', 'name', 'salary', 'age', 'email')
```


## OUTPUT
![alt text](<Screenshot 2025-04-09 215712.png>)
212224040081 DIVYASHREE B

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
