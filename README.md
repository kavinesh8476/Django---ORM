# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
### Hostel information entity diagram
![hostel](Hostel.png)

## DESIGN STEPS

### STEP 1:
Clone the repository to theia ide. start a new app inside the project folder.

### STEP 2:
Type the appropriate code for your table and provide appropriate data types to the columns.

### STEP 3:
Create a report about your project in readme.md file and upload the django.orm.app folder to your remote repository.

## PROGRAM
```
from django.db import models
from django.contrib import admin

# Create your models here.
class Hostel(models.Model):
    Roomno =models.IntegerField(primary_key=True, help_text="Roomno")
    Name =models.CharField(max_length=100)
    age =models.IntegerField()
    native =models.CharField(max_length=100)
    noofinmates=models.IntegerField()
class Hostelinfo(admin.ModelAdmin):
    list_display = ('Roomno','Name','age','native','noofinmates')
```

## OUTPUT
### Hostel info table
![output](ORM.png)

## RESULT
Thus the project is developed to have Hostel information database
