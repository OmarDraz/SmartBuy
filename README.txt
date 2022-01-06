1: Activate Environment,
- Open the project folder
- Open the terminal
- type: .\venv\Scripts\activate .. Then press enter

2: Install Requirements,
- type in terminal: 'python -m pip install -r req.txt'

3: Setup Database,
- Install PostgreSQL V.10.19 .. Set Port: 5432, Password: 123456
- Make a DB called smartbuydb
- Go to terminals and run: 'py manage.py makemigrations', 
	If there are errors:
		uninstall psycopg2 using: 'python -m pip uninstall psycopg2'
		then install it again using: 'python -m pip install psycopg2'
		then run: 'py manage.py makemigrations' again
	If there are errors still:
		uninstall Pillow using: 'python -m pip uninstall Pillow'
		then install it again using: 'python -m pip install Pillow'
		then run: 'py manage.py makemigrations' again
- Run: 'py manage.py migrate' 

4: Run the project using: 'py manage.py runserver'

The site now has no products.

5: To add Products, We have to make an admin account and navigate to our admin panel, to make that,
   run: 'py manage.py createsuperuser'
- Run the server again using: 3.4
- Navigate to 127.0.0.1:8000/admin
- Enter using username and password you have just set.
- Navigate to Products->Add->Start adding your first product!

6: Hoorraayy! The Site Now Working.