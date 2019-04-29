Django comes with ORM integrated and understanding django models is fairly easy.

Basic django model
------------------
class Product(models.Model):
    name = models.CharField(max_length=20)
    price = models.DecimalField(max_digits=10, decimal_places=2)


This create product table in the database. Every django model will create id field by default and the id will be primary_key for the table/class.


Model functions
---------------

Model managers
--------------

Django model CRUD operations
----------------------------

Django signals
--------------