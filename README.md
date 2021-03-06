Welcome to MICRO-TWITTER!
===================


"micro-twitter" is a Django-based micro version of Twitter. Some other web front-end development techniques are applied as well, i.e, html, Bootstrap. The back-end database is sqlite3.

----------

DOCUMENTS
-------------
#### <i class="icon-file"></i> REQUIREMENTS
Python3.4.2, Django1.7.1, etc, see requirements.txt.


#### <i class="icon-folder-open"></i> INSTALLMENT

```
	$ git clone https://github/lszhou/micro-Twitter
	
	or
	
	$ git clone git@github.com:lszhou/micro-Twitter.git
```

#### <i class="icon-pencil"></i> USAGE


```
	$ cd micro-Twitter
	$ pip install -r requirements.txt 
	$ python manage.py migrate
	$ python manage.py runserver
```
> - open the website(chrome best) and input http://127.0.0.1:8000/

#### <i class="icon-trash"></i> SPECIFICATIONS

> **The following features are impemented:**

> - Authorization page ( http://127.0.0.1:8000/admin/ ): Django-bootstrap-admin back-stage management. For unauthenticated users, he has to use command $ python manage.py createsuperuser to create a super user account and then manage the posts. For authenticated users (current admin account is root, pass word 123), he could use python shell sqlite3 API to manage the post, i.e, delete, post, etc. All previous posts are listed. Note: The "follow/unfollow functionality is not completed."

> - User page: Shows a list of all Tweets, including posting time, content, etc.

> - Detail page: Provides all context for a single tweet. By clicking "Read More" button, the user could see all information about current tweet and all comments to it. Note: The comment feature is implemented via "duoshuo", a Chinese-based  comment system (http://duoshuo.com/). Similarly, we could  use disqus (https://disqus.com/).

> - Tweets Search. User could use the search function provided to search the previous tweets via key words.

> - The links to GitHub, Facebook are provided.

>- (Some screen shots are attached for the reference.)
