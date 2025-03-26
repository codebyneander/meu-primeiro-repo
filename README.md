# Meu Primeiro Repositório

Olá, acabei de ganhar um micro-certificado sobre o básico de Git e Github, e um dos exercícios é descrever como eu fiz esse repositório do zero.

Primeiramente, para criar um repositório, você tem duas opções:

1. Criar o repositório no github e depois criar um repositório local.
2. Ou, criar primeiro o repositório local para colocá-lo no repositório remoto (Github).

Eu criei primeiramente o repositório local no meu computador.

1. Criei uma pasta com o nome "meu-primeiro-repo"
2. Iniciei o terminal injetado na pasta, e usando o comando:

``git init``

Depois, criei um primeiro arquivo (esse repositório, de inicio, foi apenas um teste para aula prática), e o adicionei no Stage Area.

``git add index.html``

Depois, analisei como estava o stage area:

``git status``

Depois, fiz alguns testes usando os comandos ``add``, ``restore``, etc.

Depois, criei um commit, somente com o arquivo ``index.html``:
``git commit -m "Primeiro commit"``

Depois, fiz alguns testes como deletar o arquivo, criando um commit com ele deletado:

``git commit -m "Deleted index"``

 e restaurar através do commit, dessa forma:

``git checkout (id do primeiro commit) -- index.html``

Logo após, olhei o status:

``git status``

Depois, lancei esse arquivo em um novo commit:

``git commit -m "Restaured index"``

Bom, após praticar, coloquei o repositório local no repositório remoto assim:

1. ``git remote add origin https://github.com/codebyneander/meu-primeiro-repo.git``
2. ``git push -u origin master``

Depois disso, ocorreu um erro, logo percebi que era por conta do readme que estava no repositório remoto e não estava no local, então puxei os arquivos do repositório remoto para o local com o:

``git pull``

Com êxito, enviei todos os arquivos para o repositorio remoto, atualizando-o sem erros.

``git push``

The end.
