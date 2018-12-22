# Informações do projeto

O RectQuiz foi um aplicativo desenvolvido durante as 72 horas de evento do I Amapá HackFest. 
Visando a prevenção da corrupção através da aprendizagem por reforço na educação básica, ensinando
e conscientizando o aluno sobre as práticas ilicitas de corrupção, bem como de denunciar atos ilicitos em escolas.

# Informações de funcionamento

A aplicação foi escrita com Python3 e Django 2.1.

As funções encontradas no BackEnd são:

* API REST ful para o aplicativo móvel escrito em ReactNative consumir
* Painel Administrativo para Cadastro de Questoes
* Painel de Estatísticas 
* Painel de Visualizaço de Denúncias

Além disso, esta aplicação conta com a página de home de um site construído para apresentar a ferramenta. Incluindo:

* Página home
* Página de Politicas de Privacidade
* Página de Termos de Uso
* Página de apresentação da equipe


# Requisitos

Para facilitar os testes, você pode apontar o `pip` para o arquivo `requirements.txt` e instalar as dependências do projeto:

```
# pip install -r requirements.txt
```

Após isso, crie um banco de dados em um SGBD de sua preferência e acesse o arquivo `settings.py` e altere as linhas 80 à 89:
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'projetoquiz',
        'USER': 'root',
        'PASSWORD': 'toor',
        'HOST': 'localhost',
        'PORT': '3306'
    }
}
```

Para testar se a conexão com o banco está funcionando corretamente, basta tentar aplicar uma migração na pasta do projeto:

```
$ python manage.py migrate
```

Depois criar um superusuário:

```
$ python manage.py createsuperuser 
```

Adiciona as informações, e quando tudo estiver ok:

```
$ python manage.py runserver
```

O Django irá rodar o servidor embutido no projeto e rodará no localhost de sua máquina, se tudo estiver ok, é só acessar a aplicação. =)


# Equipe de Desenvolvimento do BackEnd no Linkedin

* [Gabriel Silva](https://www.linkedin.com/in/bsgabrielsilva/) 
* [Alexsandra Souza](https://www.linkedin.com/in/alexsandrasouza/)

# Licensa

GPL
