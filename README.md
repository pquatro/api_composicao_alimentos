# API de Cadastro de Composição de Alimentos

Este pequeno projeto faz parte da Disciplina **Desenvolvimento Full Stack Básico** da Pós-Graduação Engenharia de Software PUC-Rio

A idéia desse projeto é apresentar o cadastro da tabela brasileira de composição de Alimentos - TACO. Nesse cadastro teremos os alimentos classificados por grupos alimentícios, com seus respectivos conjunto de macros principais (calorias, proteínas, carboidratos e gorduras). Esses dados são usados por nutricionistas para calcular uma dieta.

Esta API foi desenvolvida em Swagger e seu back-end em Python e Flask. Para o banco de dados, foi utilizado o SQLite.

---
# Como executar 
Após clonar o repositório, é necessário ir ao diretório raiz, pelo terminal, para poder executar os comandos descritos abaixo.

É fortemente indicado o uso de ambientes virtuais do tipo [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html).

Para criar o ambiente:
```
py -m venv env
```
Para ativar o ambiente:
```
.\env\Scripts\activate
```
Será necessário ter todas as libs python listadas no arquivo `requirements.txt` instaladas.
Para instalar as libs:
```
(env)pip install -r requirements.txt
```
Pode acontecer no momento de executar a API, a falta de alguma lib no projeto. Basta executar o comando abaixo para instalar alguma lib que esteja faltando:
```
(env)pip install <nome_da_lib>
```
Para executar a API  basta executar:

```
(env)flask run --host 0.0.0.0 --port 5000
```
Em modo de desenvolvimento é recomendado executar utilizando o parâmetro reload, que reiniciará o servidor
automaticamente após uma mudança no código fonte. 

```
(env)flask run --host 0.0.0.0 --port 5000 --reload
```

Abra o [http://localhost:5000/#/](http://localhost:5000/#/) no navegador para verificar o status da API em execução.

> Todos os comandos acima foram executados no sistema operacional Windows. Em Linux, alguns desses comandos tem sintaxe diferente.
