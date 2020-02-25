# www.iddpmirichmond.com
## Setup

###	Pre-requisites:
- Linux commandline knowledge
- Git Knowledge

### MAC

#### Install homebrew package manager:
- [https://brew.sh](https://brew.sh)

#### Install Python3

	$ brew install python3


#### Dowload the church-website repo 

	$ git clone git@github.com:iddpmirichmond/church-website.git

#### Create a Python3 Virtual Environment inside church-website repo

- change directory to the church-website repo

		$ cd church-website

- Create python virtual environment for the project


		$ python3 -m venv .venv


	This will create the .venv directory if it doesn’t exist, and also create directories inside it containing a copy of the Python interpreter, the standard library, and various supporting files.

- Activate the virtual environment

	
		$ source .venv/bin/activate
	

#### Install all required packages

	(.venv) $ pip install -r requirements.txt

#### Run website locally

	(.venv) $ cd mysite/
	(.venv) $ python manage.py migrate
   	(.venv) $ python manage.py runserver

#### Access your local copy
- **Website:** [http://localhost:8000](http://localhost:8000)
	- Website: 
![website.png](docs/images/website.png)
- **Admin:** [http://localhost:8000/admin](http://localhost:8000/admin)
	- Admin sign in:
![admin-login.png](docs/images/admin-login.png)
	- Admin panel
![admin-panel.png](docs/images/admin-panel.png) 

#### Shutdown local running website
- Press `control` + `c` key to shutdown local server
