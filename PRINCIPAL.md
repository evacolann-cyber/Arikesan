## Para realizar el Gráfico Interactivo en Python
```python
import plotly.express as px
import pandas as pd

df = pd.read_csv('data/processed/piura_pbi.csv')
fig = px.line(df, x='Año', y='PBI', title='Evolución del PBI de Piura (2007-2023)')
fig.show()  # Muestra el gráfico interactivo en el navegador o notebook
```

## Para realizar de Gráfico Interactivo en R
```r
library(plotly)
df <- read.csv('data/processed/piura_pbi.csv')
fig <- plot_ly(df, x = ~Año, y = ~PBI, type = 'scatter', mode = 'lines+markers')
fig  # Muestra el gráfico interactivo
```

## Variables Analizadas

| Código | Variable | Período |
|--------|----------|---------|
| 01 | Producto Bruto Interno (PBI) | 2007-2023 |
| 02 | Agricultura, ganadería, caza y silvicultura | 2007-2023 |
| 03 | Pesca y acuicultura | 2007-2023 |
| 04 | Extracción de petróleo, gas, minerales | 2007-2023 |
| 05 | Manufactura | 2007-2023 |
| 06 | Electricidad, gas y agua | 2007-2023 |
| 07 | Construcción | 2007-2023 |
| 08 | Comercio y mantenimiento de vehículos | 2007-2023 |
| 09 | Transporte y almacenamiento | 2007-2023 |
| 10 | Alojamiento y restaurantes | 2007-2023 |
| 11 | Telecomunicaciones | 2007-2023 |
| 12 | Administración pública y defensa | 2007-2023 |
| 13 | Otros Servicios | 2007-2023 |
| 14 | Régimen tributario | 2016-2021 |
| 15 | Empresas formales | 2016-2021 |

## Tecnologías Utilizadas

### Lenguajes de Programación
- **Python 3.8+**: Análisis de datos y visualizaciones
- **R 4.0+**: Análisis estadístico y gráficos especializados


### Bibliotecas Principales
```python
# Python
pandas == 1.5.0      # Manipulación de datos
matplotlib == 3.7.0  # Visualizaciones básicas
seaborn == 0.12.0    # Visualizaciones estadísticas
plotly == 5.15.0     # Gráficos interactivos
numpy == 1.24.0      # Cálculos numéricos
```

```r
# R
library(ggplot2)     # Gramática de gráficos
library(dplyr)       # Manipulación de datos
library(tidyr)       # Datos tidy
library(plotly)      # Gráficos interactivos
´´
