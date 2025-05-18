# ETL com o Pandas – Extração, Transformação e Carga de Dados

> **Observação**  
> Este projeto foi desenvolvido com base nos aprendizados obtidos no curso da Alura sobre ETL (Extract, Transform, Load), ministrado pela tutora Valquíria Alencar.  
> O objetivo principal é aplicar as etapas do processo de ETL utilizando exclusivamente a biblioteca **pandas** em **Python**.  
> Os dados utilizados referem-se às **emissões globais de CO₂ desde 1750** com granularidade por país e por tipo de fonte emissora.  
> Este notebook tem caráter educacional e visa consolidar conhecimentos fundamentais de manipulação de dados com pandas, sendo parte integrante do meu portfólio pessoal de Ciência de Dados.
---
## 📊 Estrutura dos dados

O arquivo principal (`dados_co2.csv`) contém as seguintes colunas:

- `País`: Nome do país.
- `ISO 3166-1 alpha-3`: Código internacional do país (ex: BRA, USA, CHN).
- `Ano`: Ano de referência.
- `Total`: Emissão total de CO₂ no ano (milhões de toneladas).
- `Carvão`: Emissões provenientes do uso de carvão.
- `Oléo`: Emissões provenientes do uso de óleo (combustíveis líquidos).
- `Gás`: Emissões provenientes do uso de gás natural.
- `Cimento`: Emissões decorrentes da produção de cimento.
- `Queima`: Emissões por queima de biomassa e resíduos.
- `Outro`: Outras fontes não especificadas.
- `Per Capita`: Emissões per capita em toneladas.
---

1. **Extração**:
   - Leitura dos dados diretamente do arquivo `.xlsx`.

2. **Transformação**:
   - Renomeação de colunas para padronização.
    - Criação de planilhas auxiliares:
     - `emissoes_CO2`: Planilha principal com as emissões totais por país e ano.
     - `emissoes_percapita`: Planilha com valores de emissão per capita.
     - `fontes`: Planilha detalhada por tipo de fonte (Carvão, Óleo, Gás, etc).

3. **Carga**:
   - Exportação dos dados tratados para arquivos Excel separados (`.xlsx`).

## 🛠️ Tecnologias Utilizadas

- Python 3.x
- pandas
- Jupyter Notebook / VS Code
- Excel / Google Planilhas


