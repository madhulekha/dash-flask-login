# dash-flask-login

![dash-flask-login](https://user-images.githubusercontent.com/31367475/47422577-4f761500-d759-11e8-90c2-b70a79fcd610.gif)

This is an example of Flask-login implementation on top of a Dash application for users authentication.

The example comes with users authentication through a sqlite3 database, however you can use your own database by changing the `con` parameter with your database URI in the `config.txt` file.

The example comes with the a standard username `test` and password `test1` but you can add more users using the `add_remove_users.ipynb` jupyter notebook or the functions available in the `users_mgt.py`.

### Files description:
`add_remove_users.ipynb`: A jupyter notebook to help creating and removing users<br/>
`app.py`: The app initial screen<br/>
`config.py`: python script to initialize the configuration included in the `config.txt` file<br/>
`config.txt`: configuration file<br/>
`requirements.in`: input configuration file to be used together with pip-tools<br/>
`requirements.txt`: configuration file generated bypip-tools<br/>
`server.py`: the app initialization file<br/>
`users.db`: sqlite3 database with user information<br/>
`users_mgt.py`: helper file for the user management process<br/>

### Running an app locally

To run an app locally:

1. (optional) create and activate new virtualenv:

```
pip install virtualenv
virtualenv venv
source venv/bin/activate
```

2. `pip install -r requirements.txt`
3. `flask run`
4. open http://127.0.0.1:5000 in your browser

### Contributing

PRs accepted! Please contribute if you believe this example can be improved.
