# Dolar_historico
```markdown
# 📈 Notebook de Extração e Visualização de Cotações

Este notebook replica o script `Extracao_de_dados_para_uma_tabela.py` utilizando a biblioteca `pandas`. Ele realiza a extração de cotações via API, grava os dados em um banco SQLite (`cotacoes.db`) e gera visualizações temporais com `matplotlib` e `seaborn`.

## ⚙️ Funcionalidades

- 🔄 Requisição à API e transformação dos dados em um `DataFrame` pandas
- 📅 Conversão da coluna de datas para o formato datetime
- 📊 Geração de gráfico da cotação de venda ao longo do tempo
- 📉 Adição opcional de média móvel à série temporal
- 💾 Salvamento dos dados em banco SQLite ou CSV de fallback
- 🖼️ Exportação da figura gerada

## 🧰 Requisitos

- Python 3.8+
- pandas
- matplotlib
- seaborn
- requests
- sqlite3 (nativo do Python)

Instale as dependências com:

```bash
pip install pandas matplotlib seaborn requests
```

## 🚀 Como Executar

1. Abra o notebook no Jupyter ou VS Code.
2. Execute as células na ordem indicada:
   - Requisição à API
   - Criação e transformação do DataFrame
   - Visualização da série temporal
   - Salvamento dos dados e da figura

## 📁 Saídas

- `cotacoes.db`: banco SQLite com os dados extraídos
- `cotacoes.csv`: arquivo CSV gerado em caso de fallback
- `grafico_cotacoes.png`: imagem da série temporal gerada

## 📌 Observações

- Certifique-se de que a API está acessível no momento da execução.
- A média móvel pode ser ajustada modificando o parâmetro `window` no código.

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se livre para usar e modificar.
