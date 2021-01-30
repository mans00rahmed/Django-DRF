## DJANGO REST FRAMEWORK - DRF

#Requirements
REST framework requires the following:

- Python (3.5, 3.6, 3.7, 3.8, 3.9)
- Django (2.2, 3.0, 3.1)
We highly recommend and only officially support the latest patch release of each Python and Django series.

#The following packages are optional:

- PyYAML, uritemplate (5.1+, 3.0.0+) - Schema generation support.
- Markdown (3.0.0+) - Markdown support for the browsable API.
- Pygments (2.4.0+) - Add syntax highlighting to Markdown processing.
- django-filter (1.0.1+) - Filtering support.
- django-guardian (1.1.1+) - Object level permissions support.

#Installation
-Install using pip, including any optional packages you want...

-pip install djangorestframework
-pip install markdown       # Markdown support for the browsable API.
-pip install django-filter  # Filtering support
...or clone the project from github.

-git clone https://github.com/encode/django-rest-framework
-Add 'rest_framework' to your INSTALLED_APPS setting.

INSTALLED_APPS = [
    ...
    'rest_framework',
]
If you're intending to use the browsable API you'll probably also want to add REST framework's login and logout views. Add the following to your root urls.py file.

urlpatterns = [
    ...
    path('api-auth/', include('rest_framework.urls'))
]

Note that the URL path can be whatever you want.
