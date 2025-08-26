
# Análise de Dados de Carros - 2025

Este projeto realiza uma análise exploratória de um conjunto de dados de veículos usados, com foco em métricas como preço, idade, condição e tipo de combustível. Os dados estão disponíveis no arquivo `carros_2025.csv`.

## 📊 Objetivos
- Entender a distribuição de preços dos veículos
- Avaliar a quilometragem média por tipo de combustível
- Analisar a idade média por tipo de carroceria
- Verificar a correlação entre idade e preço
- Explorar a influência da condição do carro no valor de venda

## 🧮 Métricas Calculadas
- Média e mediana de preço por condição
- Total de carros por condição
- Correlação entre idade e preço

## 📈 Visualizações
- Gráfico de barras: Total de carros por condição
- Boxplot: Preço por condição
- Gráfico de dispersão: Idade vs Preço com linha de tendência
- Gráfico de barras duplas: Média e Mediana de Preço por Condição

## 📦 Arquivos
- `carros_2025.csv`: Base de dados original
- `modelo_powerbi.xlsx`: Arquivo com medidas agregadas para uso no Power BI
- Gráficos gerados: disponíveis na pasta `images/`

## 🛠️ Como usar no Power BI
1. Importe o arquivo `modelo_powerbi.xlsx`
2. Crie visualizações com base nas medidas:
   - `Média Preço = AVERAGE(carros_2025[preço])`
   - `Mediana Preço = MEDIAN(carros_2025[preço])`
   - `Total Carros = COUNT(carros_2025[condição])`
   - `Correlação = CORREL(carros_2025[idade], carros_2025[preço])`
3. Adicione segmentações por país, tipo de combustível, tipo de carroceria e ano

## 📌 Requisitos
- Python 3
- Bibliotecas: pandas, matplotlib, seaborn, openpyxl

## 📚 Licença
Este projeto está sob a licença MIT.
