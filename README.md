# Django-BookStore
-----------------
## This is a simple Bookstore built using Django, Docker, HTML, CSS

the project is set up using docker container on a virtual envoirnment  
switched the default database "SQLite" to *PostgreSQL* using *psycopg2*
the first app is accounts app  
created custom users with UserCreationForm with feilds (email, username)  
added it as a AUTH_USER_MODEL in django settings  
created user unit-tests  
the second app is pages app  
the first page is a home page with a unit-tests  
created templates that contains all registrations HTML pages  
the home page checks if you are authenticated if not it redicrts you to the login page  
the login page has a form with post method that gets you login credentials  
user signup with the CustomUserCreationForm we created early  
when signing up it redirects you to login with reverse_lazy function  
it is useful for when you need to use a URL reversal before your project’s URLConf is loaded  
created unit tests for all users operations  
sending an email confimation when sign up  
the third app is books app  
created book model that has a title, author, price  
created books folder in templates it has  
book_details contains details about specific book
book_list contains a list of all availlable books  
Reviews model it connects to books using ForeignKey  
Added search that can gets the results from book list
