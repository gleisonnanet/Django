# urls.py DA PASTA DO PROJETO
  
from django.contrib import admin
from django.urls import include, path

urlpatterns = [
    path('admin/', admin.site.urls),
    path('todo/',include('app.urls')),
]
