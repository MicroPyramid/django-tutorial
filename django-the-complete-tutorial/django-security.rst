Debug=False
-----------
always run application with debug=False. Make sure of it or it will expose all internal settings to users on any error leading to severe security breach.

ENV variables
-------------
storing api keys and other sensitive data in setting file makes it easy but at a cost of inposing unwanted risk. The best way is to load such from ENV so you can have production credentials not know to normal developers.

It can be done as following

TODO: explain the above.

Never expose object IDs
-----------------------
its good practice to hide object IDs with slugs or 


CSRF
----
Always use CSRF to fight spammers


Captcha
-------
Captcha can be annoying but it adds extra layer of protection to fight spammers who can crack CSRF too.