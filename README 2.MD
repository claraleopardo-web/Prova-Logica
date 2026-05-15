📈 Análise Comparativa de Ações Brasileiras
📌 Sobre o Projeto

Este projeto apresenta uma análise financeira comparativa de importantes ações brasileiras utilizando Python e dados históricos do Yahoo Finance.

O notebook realiza análises das seguintes empresas listadas na B3:

Vale S.A. (VALE3.SA)
Ambev S.A. (ABEV3.SA)
Itaú Unibanco (ITUB4.SA)
Banco do Brasil (BBAS3.SA)
Petrobrás (PETR4.SA) como exemplo de referência

O período analisado vai de janeiro de 2023 até maio de 2026.

🧠 Objetivo

O objetivo do projeto é demonstrar como realizar:

Coleta de dados financeiros via API
Tratamento de dados com Pandas
Visualização gráfica com Matplotlib e Seaborn
Comparação de desempenho entre ações
Análise exploratória de preços históricos
🛠️ Tecnologias Utilizadas
Python
Jupyter Notebook
Pandas
Matplotlib
Seaborn
yFinance
📦 Instalação

Clone este repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git

Acesse a pasta do projeto:

cd seu-repositorio

Instale as dependências:

pip install yfinance pandas matplotlib seaborn
▶️ Como Executar

Abra o notebook no Jupyter:

jupyter notebook

Depois execute o arquivo:

AdminAnáliseAções.ipynb
📊 Estrutura da Análise

Cada análise segue as etapas abaixo:

1. Coleta dos Dados

Os dados históricos são obtidos diretamente do Yahoo Finance utilizando a biblioteca yfinance.

Exemplo:

import yfinance as yf


dados = yf.download("VALE3.SA", start="2023-01-01", end="2026-05-14")
2. Tratamento dos Dados

Os dados são organizados utilizando Pandas para facilitar a análise.

Exemplo:

import pandas as pd


print(dados.head())
3. Visualização Gráfica

Os gráficos são gerados com Matplotlib e Seaborn.

Exemplo:

import matplotlib.pyplot as plt


plt.plot(dados['Close'])
plt.title('Preço de Fechamento')
plt.show()
📈 Empresas Analisadas
Empresa	Ticker
Petrobrás	PETR4.SA
Vale	VALE3.SA
Ambev	ABEV3.SA
Itaú Unibanco	ITUB4.SA
Banco do Brasil	BBAS3.SA
📌 Possíveis Análises Futuras

O projeto pode ser expandido para incluir:

Médias móveis
Indicadores técnicos
Volatilidade
Correlação entre ativos
Retorno acumulado
Previsão com Machine Learning
Dashboard interativo
📚 Aprendizados

Este projeto ajuda a desenvolver conhecimentos em:

Ciência de dados
Análise financeira
Programação em Python
Visualização de dados
Manipulação de séries temporais
🤝 Contribuição

Contribuições são bem-vindas.

Para contribuir:

Faça um fork do projeto
Crie uma branch
Faça suas alterações
Envie um pull request
📄 Licença

Este projeto é destinado para fins educacionais.

👩‍💻 Autora

Projeto desenvolvido por Clara.
