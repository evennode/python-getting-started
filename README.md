# python-getting-started

A bare Python app, which can be deployed to [EvenNode](http://www.evennode.com) and will 
get you started with Python apps.

## Running Locally

Make sure you have [Python](http://install.python-guide.org) installed.

```sh
$ git clone git@github.com:evennode/python-getting-started.git
$ cd python-getting-started

$ pip install -r requirements.txt
$ python manage.py collectstatic

$ gunicorn gettingstarted.wsgi
```

Your app should now be running on [localhost:8000](http://localhost:8000/).

## Deploying to EvenNode

In order to deploy to EvenNode you need to create a new Python app with [EvenNode](http://www.evennode.com).  
When your app is created, you can use FTP deployment or git to deploy your app. 
For more information about deployment visit our [documentation](http://www.evennode.com/docs).
The following code helps you deploy via git.  

```sh
$ git clone git@github.com:evennode/python-getting-started.git
$ cd python-getting-started
```

Lookup the git repository name listed on the "Information" tab of your app in 
EvenNode's [web console](https://admin.evennode.com) to add a remote git repository.

```sh
$ git remote add evennode git@git.evennode.com/your-app-repository-here.git
```

Deploy app to EvenNode.

```sh
$ git push evennode master
```

## Documentation

For more information about using Python on EvenNode, see our documentation:

- [Python on EvenNode](http://www.evennode.com/docs/python)
