Views are python functions or classes to serve web requests. We map url to view function in urls.py or other related url files.

a basic django view look like this

from django.http import HttpResponse

def index(request):
    return HttpResponse("Hello")

a little more complex one would be getting parameter from url to pocess or show relevant information for exampple we want to display product information fo product id=15 then url could be something like http://<domain>/product/15/

we write url like the following
url('^product/<product_id>/$', view.function_name, name="display_product"),

view could be like the following

def display_product(request, product_id):
    product = Product.objects.get_or_404(id=product_id)
    return HttpResponse("seelcted product = " + product.name)

django decorators
-----------------