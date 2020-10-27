# ecommerce

**1. Instalasi Django**
   -   
   `pip install django`

    SETTING PROJECT BARU
   - membuat admin control project
   
     `django-admin startproject ecommercePy`

   - Menambahkan main project directory (store)
     
     `cd ecommercePy`
     
     `python manage.py startapp store`
     
   - Menambahkan directori 'store' ke settings.py
     
     Masuk ke settings.py, INSTALLED_APPS=, tambahkan
     
     `store.apps.StoreConfig`
     
   - Menjalankan server
     
     `python manage.py runserver`
     
     
**2. Setup Template & pengaturan URL**
- 
   - di dir _store_ buat dir dan sub dir baru bernama _templates_ >_store_
   - di dalam _store_, buat file html. - _store.html, main.html, cart.html, checkout.html_
   - Mengatur tampilan pada **views**
     masuk ke views.py, lalu tambahkan:
     
     `def store(request):`
     
       `context = {}`
       
       `return render(request, 'store/store.html', context)`
      
      demikian juga untuk halaman yang lain
      
   - Menambahkan urls.py pada dir store
   
     masuk kedalam dir store, lalu buat urls.py, tambahkan _urlpatterns_ (liat code)
     
   - Mendaftarkan store.urls pada ecommercePy
     
     Masuk ke ecommercePy>urls.py
     
     tambahkan pada urlpatterns:
     
     _lihat code_
     
     
       