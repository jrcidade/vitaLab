# vitaLab - Projeto de Laboratório

> Este documento vai orientar a baixar e a rodar o projeto
<br />

- `Django`, documentação: https://docs.djangoproject.com/en/4.2/
- `Pillow`, documentação https://pillow.readthedocs.io/en/stable/
- `Sqlparse`, documentação: https://sqlparse.readthedocs.io/en/latest/

### 1º Etapa: baixar o repositorio do github
    $ git clone git@github.com:jrcidade/vitaLab.git
    $ cd vitaLab

### 2º Etapa: criar uma virtualenv e ativar o ambiente venv
    $ python -m venv venv
    $ source venv/bin/activate

### 3º Etapa: instalar os pacotes do projeto
    $ pip install -r requirements.txt

### 4º Etapa: criar o banco de dados
    $ python manage.py migrate

### 5º Etapa: criar o superUsuario
    $ python manage.py createsuperuser

### 6º Etapa: Executar o projeto
    $ python manage.py runserver
O Endereço da aplicação é: http://127.0.0.1:8000/

<h1>Estrutura do código</h1>

O projeto é codificado utilizando uma estrutura simples e intuitiva apresentada a seguir:

```bash
< VITALAB >
|
|-- exames/                     # APP exames
|
|-- templates/                  # TEMPLATE
|       |-- bases/
|             |-- base.html
|       |-- static/
|             |-- geral
|             |-- usuarios
|
|-- usuarios                    # APP usuarios
|
|-- vitalab/
|       |-- settings.py         # Configurações do projeto
|       |-- urls.py             # Urls do projeto
|
|-- .gitignore                  
|
|-- manage.py                   # Script de início padrão do Django
|
|-- requeriments.txt            # Dependências do Projeto
|
|-- ****************************************************************
```


