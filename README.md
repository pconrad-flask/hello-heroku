# hello-heroku
Minimal hello world webapp deployable on Heroku 


# Dependencies

You will need to use "pip install ..." to install these modules

```
pip install flask
pip install gunicorn
```

# To run locally

You should run from the command line, not from inside IDLE

```
$ export FLASK_APP=hello.py
$ python -m flask run
 * Running on http://127.0.0.1:5000/
```

Then put a web browser to `http://127.0.0.1:5000/`

# The minimal files you need to deploy to Heroku

| What you need | Why you need it | Example |
|---------------|-----------------|---------|
| `hello.py` | So there's something to run | [hello.py](hello.py) |
| `requirements.txt` | Tells Heroku that this is a Python application, and which `pip` modules to install (i.e. what the dependencies are) | [requirements.txt](requirements.txt) |
| `Procfile` | Tells Heroku that this is a webapp, and which Python file to load, and which Python object to load as the app | [Procfile](Procfile) ||


# To deploy to Heroku

There are several ways to do it.  Here is a way that does not
require first downloading the Heroku CLI:

* Create a free tier account at Heroku.com
* Create a a new app
* Under deploy, select Github, and connect the heroku app to the repo
* Click button to `Enable Automatic Deploys`
* Click button to `Deploy Branch` deploying the master branch
* Watch under `Activity` as it loads the application
* Click the `Open` button to open the application's page

