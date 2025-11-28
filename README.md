# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 5 Car 

## PROGRAM

models.py

from django.db import models
from django.contrib import admin
class product(models.Model):
    name=models.CharField(max_length=100)
    batch_number=models.IntegerField()
    product_id=models.IntegerField()
    manufacture_date=models.DateField()
    price=models.IntegerField()
    product_id=models.IntegerField(primary_key=True)
    colours=models.CharField(max_length=20)
class productAdmin(admin.ModelAdmin):
    list_display=["name","batch_number","product_id","manufacture_date","price","product_id","colours"]


admin.py

from django.contrib import admin
from .models import product,productAdmin
admin.site.register(product,productAdmin)

## OUTPUT
![WhatsApp Image 2025-11-28 at 17 28 50_beea6698](https://github.com/user-attachments/assets/efdb0884-8190-4068-933d-d17a317b357d)




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
