# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

employeelist(image/employeelist.png)

## DESIGN STEPS

### STEP 1:
first go to student.saveetha.ac.in and open theiaide

### STEP 2:
open theiaide and go to admin.py and open models.py put some comments

### STEP 3:
open github.com and create and generate classic token 

Write your own steps

## PROGRAM
python
```
class Employee(models.Model):
    emp_id=models.CharField(primary_key=True,max_length=4,help_text="Employee ID")
    ename=models.CharField(max_length=50)
    post=models.CharField(max_length=20)
    salary=models.IntegerField()
    age=models.IntegerField()


class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','salary','age')
```
python
```
from django.db import models
from django.contrib import admin
# Register your models here.
admin.site.register(Employee,EmployeeAdmin)
```


# Create your models here.




## OUTPUT

employelist(image/employeedetails.png)

errorlist(image/employeeerror.png)


## RESULT
I  develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).