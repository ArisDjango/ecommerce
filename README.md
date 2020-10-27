# ecommerce

1. Instalasi Django
   `pip install django`

    SETTING PROJECT BARU
   - membuat admin control project
   
     `django-admin startproject ecommercePy`

   - Menambahkan main project directory
     
     `cd ecommercePy`
     
     `python manage.py startapp store`
     
   - Menambahkan directori 'store' ke settings.py
     
     Masuk ke settings.py, INSTALLED_APPS=, tambahkan
     
     `store.apps.StoreConfig`
     
   - Menjalankan server
     
     `python manage.py runserver`