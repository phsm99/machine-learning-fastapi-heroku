# Deploy ML models with FastAPI, Docker, and Heroku

### 1. Develop and save the model with this Colab

[Open Colab](https://colab.research.google.com/drive/15V8MrVJqKvSZvGnzuVV4B3jcQX0SSljy?usp=sharing)

https://www.youtube.com/watch?v=Dqltoqs5J7I

### 2. Create Docker container

```bash
docker build -t app-name .

docker run -p 80:80 app-name
```

### 3. Create Git repo

If you clone this repo this step is not needed. Or you can delete this git repo with `rm -rf .git` and start with a new one:

```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
```

### 4. Create Heroku project

```bash
heroku login
heroku create your-app-name
heroku git:remote your-app-name
heroku stack:set container
git push heroku main
```
