### How to deploy a web app in heroku
> Firt download & install heroku CLI ( command line interface)
> create heroku account
> now type the following commands
```
heroku login
```
> Initialize a git repository in a new or existing directory ( i am assuming that you are in your project root directory)
```
git init
heroku git:remote -a imdb-search-mv
git add .
git commit -am "make it better"
git push heroku master
```
###### if your project is already initialized with git then you just need to add heroku remote
```
git push heroku master
```

## How to deploy static website in heroku
just follow this link https://gist.github.com/wh1tney/2ad13aa5fbdd83f6a489

