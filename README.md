# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://user-images.githubusercontent.com/121373170/212477332-8ba731b5-dcab-4e5e-a49b-42c6adb377a4.png)

## DESIGN STEPS

### STEP 1:
creating a table using patient details in ORM

### STEP 2:
upload the python code

### STEP 3:
push the code to github

## PROGRAM

```
admin.py:

from django.contrib import admin
from .models import Studentdetail,StudentdetailAdmin


admin.site.register(Studentdetail,StudentdetailAdmin)
# Register your models here.


models.py:

from django.db import models
from django.contrib import  admin


#Create your models here.
#Create your models here.
# Create your models here.
class Studentdetail(models.Model):
    referencenumber = models.CharField(max_length=10, primary_key=True , help_text="your reference no ")
    name= models.CharField(max_length=100)
    department = models.CharField(max_length=200)
    age=models.IntegerField()
    email=models.EmailField()
class StudentdetailAdmin(admin.ModelAdmin):
    list_display = ('RefNum', 'Name', 'Age', 'Email','Dept')
```

## OUTPUT

![image](https://user-images.githubusercontent.com/121373170/212480249-a3203e5b-d805-457c-a3d6-a1bcccad3706.png)


## RESULT
Thus the experiment was executed successfully.
