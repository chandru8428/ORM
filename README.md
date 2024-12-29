# Ex02 Django ORM Web Application
# Date:13-11-2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py

from django.contrib import admin
from .models import bankloan,userAdmin
admin.site.register(bankloan,userAdmin)

models.py

from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    customer_name=models.CharField(max_length=100,primary_key=True)
    customer_id=models.CharField(max_length=100)
    loan_no=models.IntegerField()
    loan_amount=models.IntegerField()
    email=models.EmailField()
 
class userAdmin(admin.ModelAdmin):
    list_display=('customer_name','customer_id','loan_no','loan_amount','email')


```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot 2024-12-06 212909](https://github.com/user-attachments/assets/b20a788c-024b-49fe-b5ef-6701d3b0dfe6)
![WhatsApp Image 2024-12-19 at 13 58 45_5d0c163e](https://github.com/user-attachments/assets/e935a768-1abd-4720-9a33-638ff47dffc0)
![image](https://github.com/user-attachments/assets/2abd5f72-2433-45c0-8e79-e30073324939)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
