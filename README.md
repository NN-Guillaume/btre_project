All credits of this project goes to Brad TRAVERSY
Link to his Udemy account: https://www.udemy.com/user/brad-traversy/
Link to his YouTube channel: https://www.youtube.com/channel/UC29ju8bIPH5as8OGnQzwJyA

--------------------------------------------------------------

Cloning Django Project

Step by step

--------------------------------------------------------------

01 - Clone the repo on github to vscode

02 - Create the virtual env and activate it
	execute --->	virtualenv -p python3 venv
		--->	./venv/scripts/activate

03 - Install the dependencies (requirements.txt)
	execute --->	pip install requirements.txt

04 - Might need to generate a new django secret key
	file " .env " where to store the key
	you can copy your own key
	google the process if it oesn't works

05 - Create the database
	first, install postgres + pgadmin if not done
	create the db on pgadmin

06 - Check the file settings.py
	---> HOST ? (the one you set to pgadmin)
	---> PASSWORD ? (the one you set to pgadmin)
	---> ALLOWED_HOSTS ? (certainly '127.0.0.1')

07 - execute --->	Python manage.py makemigrations

08 - execute --->	Python manage.py migrate

09 - Check on pgadmin if the tables are created

10 - execute --->	Python manage.py runserver

It works ! congrats ! You can start working on it !   ;-D