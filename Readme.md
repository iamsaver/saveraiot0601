# AIoT Github
<br>

##### auther :Saver

## Lecture 15: IoT Flask Web (deploy to heroku)

### step 0 : Setup Environment
* github、heroku sign up
* install HeidiSQL、VS code

### step 1 : Clone this github

。把local的 \aiot0531.git 殺掉 (產生自己的git管理員) 方便建立新的git repository
。推送至github 建立新的 saver_0601 https://github.com/iamsaver/saveraiot0601

### step 2 : install some package
* if you want to test locally,you need to install the following packages(That is the same thing in the requirements.txt)

```python
pip insall gunicorn   
Flask==2.0.1 
Jinja2==3.0.1 
psycopg2 
sklearn 
pandas  
numpy 
```

### step 3: add an heroku postgredb

* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb

### step 4: login to heroku pstgredb using HeidiSQL


```sql
myserver ="<ec2-34-227-120-79.compute-1.amazonaws.com
>"
myuser="<alcykghivllubp
>"
mypassword="<16abea5741ee458e4972f91dc15e24d0d7ed7a5a3560e6ce80002c1dfc7955f2>"
mydb="<d8al4p5betfiku>"

```
### step 5: import postgredb (in db/postgre.db)


### step 6: setting db in app.py


```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 7: testing locally by running python app.py

### step 8: deploy to github (new private github repositoy)

delete .git and git remote add origin master github.com/xxxxx


### step 9: Heroku deploy from github

### step 10: Complete

Sample link 1:
https://awinlab-aiot.herokuapp.com/

Sample link 2: 
https://aiot0601a.herokuapp.com/





