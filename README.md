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

- acessar sonarqube e importar o projeto

- criar arquivo GCP/cloudbuild
    conectar no repositorio
    criar acionador

- github
    settings/branches
    addrule/master
    Require status checks to pass before merging
    Require branches to be up to date before merging
    Trigger: 0cd95749-107a-4690-9db5-6e4b8b37ba94
    Include administrators

- testar
    adicionar txt build
    git add .
    git commit -m 'Adicionando comentario cloudbuild'
    git push origin master

- editar GCP/cloudbuild
    alterar acionador para evento solicitacao pull

- criar o branch de trabalho
    git checkout -b teste
    git push origin teste

- criar pull request
    no site do github

- (github) adicionar pessoas a organizacao
    edit rule do branch
    Require pull request reviews before merging

- criar pull request
    no site do github
    git add .
    git commit -m 'Adicionando comentario de Migracao'
    git push origin teste



