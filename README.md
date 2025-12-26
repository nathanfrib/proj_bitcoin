# Monitoramento de Preços do Bitcoin

Este projeto é uma aplicação em Python desenvolvida para monitorar o preço do Bitcoin utilizando a API pública da Binance. Os dados obtidos são registrados em um banco de dados SQLite3 para análise e visualização posterior.

## Funcionalidades

- **Monitoramento em Tempo Real:** Busca os preços do Bitcoin em intervalos regulares usando a API pública da Binance.
- **Registro em Banco de Dados:** Armazena os dados de preço em um banco de dados SQLite3 para armazenamento persistente.
- **Intervalos Configuráveis:** Permite a personalização dos intervalos de monitoramento.

!["Bitcoin ETL"](image/etl_bitcoin.png)

## Pré-requisitos

Antes de executar o projeto, certifique-se de ter os seguintes requisitos instalados:

- **Python 3.8+**
- Bibliotecas Python: `requests`, `sqlite3`, `pandas`

## Instruções de Configuração

### 1. Clone o Repositório

```bash
git clone https://github.com/nathanfrib/proj_bitcoin.git
cd proj_bitcoin
```

### 2. Instale as Dependências

Crie um ambiente virtual e instale os pacotes Python necessários:

```bash
python -m venv .venv
source .venv/bin/Activate  
pip install -r requirements.txt
```
### 3. Execute a Aplicação

Inicie a aplicação com:

```bash
python main.py
```

## Como Usar

1. O script buscará o preço do Bitcoin periodicamente e registrará os dados no banco de dados SQLite3.
2. Você pode consultar o banco de dados para analisar as tendências de preço ou integrar os dados em outras aplicações.

## Estrutura do Projeto

```plaintext
proj_bitcoin/
├── main.py          # Script principal
├── requirements.txt # Dependências do Python
└── README.md        # Documentação do projeto
```

## Dependências

O projeto utiliza as seguintes bibliotecas Python:

- `requests`: Para realizar requisições HTTP à API da Binance.
- `sqlite3`: Para configurar e armazenar os dados em um banco SQL.
- `pandas`: Para manipulação e transformação de dados.

## Melhorias Futuras

- Adicionar suporte para monitoramento de múltiplas criptomoedas.
- Implementar uma interface web para visualização em tempo real dos preços.
- Adicionar funcionalidade de alertas para mudanças significativas no preço.

## Contribuições

Contribuições são bem-vindas! Por favor, faça um fork do repositório e envie um pull request para quaisquer mudanças ou melhorias.
