
# PYSTACK WEEK 10 <br>Aplicação de Telemedicina com Django
O projeto Healing foi concebido com o objetivo de simplificar o acesso aos cuidados de saúde, eliminando as barreiras tradicionais, como longas esperas e deslocamentos. Nossa plataforma permite que pacientes agendem consultas com especialistas de nossa clínica de forma rápida e fácil, tudo isso através do nosso site de telemedicina.
Os pacientes podem se conectar com os médicos através de videochamadas seguras e confidenciais e também os pacientes podem agendar suas consultas com especialistas da nossa clínica de maneira conveniente através da plataforma.
As consultas podem ser marcadas de acordo com a disponibilidade dos médicos e dos pacientes.
Os médicos têm acesso a uma interface intuitiva onde podem visualizar suas consultas agendadas.
<hr>

   ## Arquitetura do nosso projeto com framework Django
<center>
 
![Imagem do projeto](templates/static/geral/img/diagrama%20fluxo.png)

</center>

#### Projeto disponibilizado por:
https://pythonando.com.br/
<br>
https://www.youtube.com/@pythonando

## Após Clonar o repositório, Seguir as seguintes etapas abaixo:


## Preparação do ambiente
Estou desenvolvendo no ambiente windows. 



## Configurações
 Python versão ^3.10

### Para Iniciar um ambiente windows
````
python -m venv venv
````

#### Caso algum comando retorne um erro de permissão execute o código e tente novamente:
- Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

### Após a criação do venv vamos ativa-lo:

````
venv\Scripts\Activate
````

### Agora vamos fazer a instalação do Django e as demais bibliotecas:

````
pip install django
pip install pillow
````
## Vamos criar o nosso projeto Django:
````
django-admin startproject healing 
````

### Rode o servidor para testar:
````
python manage.py runserver
````

### Criando as tabelas do banco de dados
````
Comando para criar as tabelas do banco de dados que já foram instaladas junto do projeto.

python manage.py migrate
````
### Criando as migrations
Cria um conjunto de comandos para mais tarde ser criado as tabelas no banco de dados, como se fosse uma preparação para criação das tabelas, para depois rodar o comando 'python manage.py migrate' para gerar as tabelas. 
````
python manage.py makemigrations 
````
### Comando para criar um SuperAdmin no projeto
````
python manage.py createsuperuser
````


