# Ex03 Time Table
## Date:04-04-2024

## AIM
To write a html webpage page to display your slot timetable.

## ALGORITHM
### STEP 1
Create a Django-admin Interface.

### STEP 2
Create a static folder and inert HTML code.

### STEP 3
Create a simple table using ```<table>``` tag in html.

### STEP 4
Add header row using ```<th>``` tag.

### STEP 5
Add your timetable using ```<td>``` tag.

### STEP 6
Execute the program using runserver command.

## PROGRAM
models.py
from django.db import models from django.contrib import admin class Employee (models.Model): eid=models.CharField(max_length=20,help_text="Employee ID") name=models.CharField(max_length=100) salary=models.IntegerField() age=models.IntegerField() email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin): list_display=('eid','name','salary','age','email')

admin.py
from django.contrib import admin from .models import Employee,EmployeeAdmin

admin.site.register(Employee,EmployeeAdmin)

## OUTPUT
![Screenshot 2024-04-05 093708](https://github.com/KISHORENARAYANANSR/slot/assets/148202102/8fe6d56a-1e2c-432b-81ed-1e722e39c07f)


## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
