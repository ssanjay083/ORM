# Ex02 Django ORM Web Application
# Date:19.10.2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
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
models.py
```
from django.db import models
from django.contrib import admin

class Book (models.Model):
  
    book_no=models.IntegerField()
    book_name=models.CharField(max_length=100)
    author_name=models.CharField(max_length=100) 
    Email=models.EmailField()
    buyer_name=models.CharField(max_length=100)
    mobile_no=models.IntegerField()

class BookAdmin(admin.ModelAdmin):
    	list_display= ('book_no', 'book_name', 'author_name', 'Email', 'buyer_name','mobile_no')
```
views.py
```
from django.contrib import admin
from django.urls import path

urlpatterns = [
    path('admin/', admin.site.urls),
]
```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot 2024-12-07 135324](https://github.com/user-attachments/assets/66e7cdd6-3401-4f2d-9aba-92c0f87cdbe5)
![Screenshot 2024-12-07 135511](https://github.com/user-attachments/assets/1bfb0043-7d37-4d1b-8c77-feeb8f6f8e39)
![Screenshot 2024-12-07 135618](https://github.com/user-attachments/assets/d97f83fd-28ed-45cf-900c-1e8d9a1cfe7a)
![Screenshot 2024-12-07 135733](https://github.com/user-attachments/assets/65c36169-1892-4a10-ad65-b33362e20ead)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
