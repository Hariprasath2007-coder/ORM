# Ex02 Django ORM Web Application
# Name:HARI PRASATH E
# Ref No: 25007799
## Date: 14-09-2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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

models.py
```
from django.db import models
from django.contrib import admin
class Car(models.Model):
    car_id=models.IntegerField(primary_key=True)
    brand=models.CharField(max_length=20)
    car_model=models.CharField(max_length=20)
    cos_email=models.EmailField()
    dop=models.DateField()
class CarAdmin(admin.ModelAdmin):
    list_display=['car_id','brand','car_model','cos_email','dop']
```

admin.py
```
from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)

```


## OUTPUT


<img width="1908" height="974" alt="Screenshot 2025-09-21 154854" src="https://github.com/user-attachments/assets/09215340-5445-499e-ad8e-1f9729329748" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
