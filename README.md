# STEPS TO CREATE AND DEPLOY THE WEBSITE

## Python Flask Website (using Visual Code)

1) Create script1.py
2) Create templates folder
3) In templates folder create html files
4) Run .\script1.py in python terminal "python .\script1.py"
5) Move all the folder into new folder
6) open VS Code in New Folder install virtual environment 
		"pip install virtualenv"
		"python -m venv virtual"
7) Install flask "virtual\Scripts\pip install flask"
8) Optional - "virtual\Scripts\python.exe -m pip install --upgrade pip"
9) Run the app - "virtual\Scripts\python Portfolio\script1.py"

## Python website deployment
## Heroku

1) Create Heroku account
2) Download herokutoolbelt 
3) Go to Script1.py location and open Poweshell or CMD
4) In Cmd Line type "heroku login" and login 
5) to create app "heroku create <appname>"
6) Go to following url 

7) Take list of packages in virtual env "..\virtual\Scripts\pip freeze"
8) Install gunicorn for https purpose -->PS D:\mysite\Portfolio> "..\virtual\Scripts\pip install gunicorn"
--Create 3 files "requirement.txt","Procfile","runtime.txt"
9) Create requirement.txt file in normal folder D:\mysite\Portfolio> "..\virtual\Scripts\pip freeze > requirements.txt"
10) Create Procfile without any extensions "web: gunicorn script1:app"
11) Check python version of app and also check in the heroku supported runtime
	Check python version - "python -V"
	runtime.txt file should contain - "python-3.8.5"
	
12) Create Git Repo - "git init"
13) Add all files in git "git add ."
14) Commit files to Git using this cmd "git commit -m "first commit" "
15) before pushing to heroku point to corresponding app in heroku using "heroku git:remote --app ebcdstest" in cmd 
16) config git to ur heroku email used 
		"git config --global user.email "<email>" "
		"git config --global user.name "<username>" "
17) Push the changes to Heroku with "git push heroku master"
18) Success message "remote: Verifying deploy... done." if the commit was successful
19) open ur app using cmd by "heroku open" or by copying the web link 
20) app info using cmd "heroku info"

## References:
1) https://www.hongkiat.com/blog/
2) https://www.dataquest.io/blog/how-to-setup-a-data-science-blog/
3) https://www.w3schools.com/
4) https://startbootstrap.com/
5) https://unsplash.com/
