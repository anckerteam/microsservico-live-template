# microsservico-live-template

 passos:

- crio os arquivos necessários
    requirements.txt
    Dockerfile
    docker-compose.yaml

- rodar o docker-compose para criar a estrutura do django
    docker-compose run web django-admin startproject codeprogress .

- testar
    docker-compose up -d
    docker-compose ps
    docker exec -it codeprogress_app bash
        python3 manage.py migrate

- ajustar arquivos
    .gitignore

- criar repo no github e 
    git init
    git remote add origin https://github.com/anckerteam/microsservico-live-template.git add .
    git commit -m "first commit"
    git push -u origin master

