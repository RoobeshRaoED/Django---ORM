# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![](Entity%20relationship%20diagaram.png)

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM

```
admin.py:  

from django.contrib import admin  
from .models import Student,StudentAdmin  


admin.site.register(Student,StudentAdmin)  

manage.py:  

from django.db import models  
from django.contrib import admin  
#Create your models here.  

class Student(models.Model):  
    referencenumber=models.CharField(max_length=10,help_text="Your Reference Number")  
    name=models.CharField(max_length=100)  
    department=models.CharField(max_length=200)  
    age=models.IntegerField()  
    email=models.EmailField()  

class StudentAdmin(admin.ModelAdmin):  
    list_display = ('referencenumber','name','age','department','email')  
#Register your models here.  
```

## OUTPUT

![](Roobesh%20Rao.E.D%2022008573%20user%20addition.png)


## RESULT
