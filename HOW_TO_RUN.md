#Form Validation using Testing in Python

##MUST KNOW
The project is integration of the following layers

* The user interface (HTML/CSS),
* Middleware (Flask), and
* Database (SQLite).

##BEFORE RUNNING THE PROJECT PLEASE RUN THE FOLLOWING LINE ON TERMINAL/CMD/...

pip install -r requirements.txt

## Starting the server locally to interact with the Survey Form

1. In your terminal, type `flask run`

2. Either click on the link provided in your terminal `http://127.0.0.1:5000/`

   or insert it directly on your web browser.

## Fill and submit the form

1. Fill all the values in the form

2. Name and email are required values

3. Click on submit, at which point you *should* receive a "Your form was submitted" message in red.

## Running the User Interface tests
##NOTE: OPEN ANOTHER TERMINAL, WHILE THE LOCAL SERVER IS RUNNING
1. Make sure your local server is running.
2. Alternatively, you can run the file directly, typing: `python3 test_survey_ui.py`
3. And WAIT, let it run... It runs 7 tests


##As mentioned above at line #8, our projects backend is SQLite
## One can check the db again to check that it received the values from the form

1. In your terminal, type  `flask shell`

2. Run the following and check that the output is the same as the values you entered in the form.

```
>>>Voter.query.all()
>>>Answer.query.all()
>>>Language.query.all()
>>>Comment.query.all()
```





