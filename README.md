# MindPeace Habit Tracker App
This is a beginner-friendly project to help you get started with your hacktoberfest. If you don't know where to start, feel free to watch the videos linked below, and read the contribution rules. Happy hacking <3 💙 !!

P.S. Star ⭐ and Share this repository, if you had fun!! 😍

# 📌 Videos 📽️:

- [Hacktoberfest Intro](https://www.youtube.com/watch?v=mq_FIHdxmIk)
- [How to pull request [Overview]](https://youtu.be/DIj2q02gvKs)
- [Merge Conflict / comment](https://youtu.be/zOx5PJTY8CI)


# Contribution Rules📚:

- You are allowed to make pull requests that break the rules. We just merge it ;)
- Do NOT add any build steps e.g npm install (we want to keep this a simple static site)
- Do NOT remove other content.
- Styling/code can be pretty, ugly or stupid, big or small as long as it works
- Add your name to the contributorsList file
- Try to keep pull requests small to minimize merge conflicts


## Getting Started 🤩🤗:

- Fork this repo (button on top)
- Clone on your local machine

```terminal
git clone https://github.com/fineanmol/Hacktoberfest2022.git
```
- Navigate to project directory.
```terminal
cd Hacktoberfest2022
```

- Create a new Branch

```markdown
git checkout -b my-new-branch
```
- Add your Name to `contributors/contributorsList.js`
```markdown
git add .
```
- Commit your changes.

```markdown
git commit -m "Relevant message"
```
- Then push 
```markdown
git push origin my-new-branch
```


- Create a new pull request from your forked repository

<br>

## Avoid Conflicts {Syncing your fork}

An easy way to avoid conflicts is to add an 'upstream' for your git repo, as other PR's may be merged while you're working on your branch/fork.   

```terminal
git remote add upstream https://github.com/fineanmol/Hacktoberfest2022
```

You can verify that the new remote has been added by typing
```terminal
git remote -v
```

To pull any new changes from your parent repo simply run
```terminal
git merge upstream/master
```

This will give you any eventual conflicts and allow you to easily solve them in your repo. It's a good idea to use it frequently in between your own commits to make sure that your repo is up to date with its parent.

For more information on syncing forks [read this article from Github](https://help.github.com/articles/syncing-a-fork/).

## Swags of Hacktoberfest:
- Many of the candidates get attracted towards hacktoberfest to get swags . So, after 4 successfully merged pull request as for 2021 you will be eligible to get a Hacktoberfest T-shirt and Some stickers on your doorstep.


# Project Documentation 

## Description 
MindPeace Web Application is designed to help you track all your habits. Each logged in user can create and manage multiple types of trackers(like running, sleeping ,etc) and keep a note of your daily life.. The user can access all different habits from the dashboard  and can add more logs to it , add more trackers, and view their progress . 

### Technologies used 
1. flask {for application framework} 
    • Flask 
    • url_for 
    • render_template 
    • redirect 
    • request 
2. Flask_SQLAlchemy 
3. Bootstrap  
4. HTML
5. CSS
6. Matplotlib{for plotting graphs}
7. Datetime{for timestamp}

### DB Schema Design 
<b>1. User Table </b>

|Column  | Data type | Constraints       | Description|
|--------|-----------|-------------------|------------|
|id      |   Integer | Primary key       | User Id    |
|username| String(30)| Unique , not null | User Name  |
|password|String (30)| Not null          | Password   |

<b>2. Trackers</b>

|Column      | Data type | Constraints              | Description|
|------------|-----------|--------------------------|------------|
|id          | Integer   | Primary Key              |     Id     |
|name        | String(30)| Not null                 |Tracker Name|
|description |String(100)|       -                  | Description of tracker type|
|last_update | DateTime  | Not null                 | When was tracker last updated|
|user_id     | Integer   | Foreign Key from User    |  User Id Table, Not Null|

<b>3. Logs</b>

|Column      | Data type | Constraints                   | Description|
|------------|-----------|-------------------------------|------------|
|id          | Integer   | Primary Key                   |     Id     |
|when        | DateTime  |       -                       | When was this log added|
|value       | Float     |   Not null                    | Value that we want to add in log|
|notes       | String    |       -                       | Any remarks about the log|
|tracker_id  | Integer   | Foreign Key from tracker Table| Tracker id|



### Architecture and Features 

The main control of the application is in file ‘main.py’. 
The template folder contains all the html files. 
The static folder contains css style sheets and the ‘images‘  folder which contains images  used in the project. 
‘trackdb.sqlite3’ contains the database. 
<br><br> 
## Submitted by: 
#### <a href="github.com/archit-1203"> ARCHIT SRIVASTAVA </a>
## Contributors: 
#### Maintainer: <a href="github.com/kushagrathisside"><b>KUSHAGRA SRIVASTAVA</b></a> 
#### Other contributors: 
<a href="https://github.com/MYCIN-AI-Club/MindPeace-WebApp/graphs/contributors"> <img src="https://contrib.rocks/image?repo=MYCIN-AI-Club/MindPeace-WebApp" /> </a>
