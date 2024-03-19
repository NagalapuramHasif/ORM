# Ex02 Django ORM Web Application
## Date: 19.03.2024

## AIM
To develop a Django application to store and retrieve data from a Railway database using Object Relational Mapping(ORM).
## Entity Relationship Diagram


![WhatsApp Image 2024-03-19 at 10 08 02_256f6f8a](https://github.com/NagalapuramHasif/ORM/assets/149365567/7a837c64-5fcb-45f4-b94f-08c99fd827e3)
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
from django.contrib import admin

from .models import Train, TrainAdmin

admin.site.register(Train, TrainAdmin)

models.py


from django.db import models
from django.contrib import admin
class Train(models.Model):
    Train_code=models.CharField(max_length=20,primary_key=True)
    Train_name=models.CharField(max_length=100)
    start_time=models.DateTimeField()
    End_time=models.DateTimeField()
    start_station_code=models.CharField(max_length=20)
    End_station_code=models.CharField(max_length=20)
 
class TrainAdmin(admin.ModelAdmin):
    list_display=('Train_code','Train_name','start_time','End_time','start_station_code','End_station_code')

```

## OUTPUT
![WhatsApp Image 2024-03-19 at 09 57 51_78ff9fc0](https://github.com/NagalapuramHasif/ORM/assets/149365567/29e0cdf8-924e-4df7-9909-fb80cf536854)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
