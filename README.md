<h1 align="center"> Analise_Dados "Vendas" </h1>

![img-Dados](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/39d8c892-347e-4a4a-ad4a-43311d52b248)

<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=%20CONCLUIDO&color=GREEN&style=for-the-badge"/>
</p>
<p align="center">
<img loading="lazy" src="https://img.shields.io/github/stars/torquato-sys?style=social"/>
</p>

* [Descrição do Projeto](#descrição-do-projeto)
* [Funcionalidades e Demonstração da Aplicação](#funcionalidades-e-demonstração-da-aplicação)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Pessoas Desenvolvedoras do Projeto](#pessoas-desenvolvedoras-do-projeto)


# Descrição do Projeto

## Projeto realizado através das aulas Hashtag Treinamentos LTDA, estamos utilizando 4 Bibliotecas para tornar tudo isso possivel.
* Biblioteca OS
* Biblioteca Pandas as pd
* Biblioteca glob
* Biblioteca plotlyb.express as px

## Utilizamos a biblioteca glob para concluir o codigo pois pandas estava apresentando erro ao tentar mesclar 5 planilhas e tornar uma só.
## Codigo utilizado anteriormente:
```ruby
tabela_total = pd.DataFrame()

for arquivo in lista_arquivo:
    if "Vendas" in arquivo:
       tabela = pd.read_csv(f"Vendas/{arquivo}")
       tabela_total = tabela_total.append(tabela)
```
### O .append() apresentava erro ao tentar adicionar os .csv no DataFrame(). Erro: Erro ao processar o arquivo Vendas - Belo Horizonte.csv: 'DataFrame' object has no attribute 'append'
### Porém com a biblioteca glob conseguimos simular a mesma coisa que o pandas iria fazer.
## Codigo com glob:
```ruby
arquivos_vendas = glob.glob('Vendas/Vendas*.csv')

lista_dataframes = []

for arquivo in arquivos_vendas:
    dataframe = pd.read_csv(arquivo)
    lista_dataframes.append(dataframe)

tabela_total = pd.concat(lista_dataframes, ignore_index=True)
```
### Aqui estamos criando uma lista simples apenas abrindo colchetes [], foi a mesma logico porém utilizando uma biblioteca a mais.


# Funcionalidades e Demonstração da Aplicação

# :hammer: Funcionalidades do projeto

- `Funcionalidade 1`: Tratamento de dados Excel
- `Funcionalidade 2`: Realizar analises de dados individual
- `Funcionalidade 2a`: Realizar contas de tabelas de forma pratica e rapida
- `Funcionalidade 3`: Gerar graficos visuais para melhor analise e uma possivel apresentação

## Listando arquivos na pasta "Vendas".
![Biblioteca os.listdir](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/94b5169a-0aa3-4ca3-a08e-4493d14e4638)

## Juntando todos os aquivos .csv com "Vendas" no nome do arquivo.
![Tabela_total](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/dfce2ba5-55e8-4257-b6c2-31044b7112fe)

## Modelando os dados com Pandas:
![modelagem_dados](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/95e51c06-5c66-4edf-b3e4-937952865c8c)
![modelagem_dados](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/59393bc7-c462-4d3c-aab9-9b53d45ab5ea)
![modelagem_dados](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/62060617-8721-4574-8221-79d8daa30f03)
![grafico](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/b167d6a3-dbed-49d2-809c-3fb00f77b42d)


# Tecnologias utilizadas
- ``Python 3.x``
- ``VSCode IDE``
- ``Jupter Notebook``
- ``Pandas``

# Pessoas Desenvolvedoras do Projeto

# Autores

[<img src="https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/8c284170-6a7e-4ca8-83b0-249bb3cb93ca" width="115">](https://github.com/torquato-sys)
<br>
<sub>Mateus Torquato Fernandes</sub>

![Banner-divulgação](https://github.com/Torquato-sys/Analise_Dados-Vendas-/assets/80015572/ea2c501f-526d-4c1c-8d69-a22571b1219e)
