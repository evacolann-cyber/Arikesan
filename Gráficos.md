## 🖱️ Ejemplo de Gráfico Interactivo en Python
```python
import plotly.express as px
import pandas as pd

df = pd.read_csv('data/processed/piura_pbi.csv')
fig = px.line(df, x='Año', y='PBI', title='Evolución del PBI de Piura (2007-2023)')
fig.show()  # Muestra el gráfico interactivo en el navegador o notebook
```

## 🖱️ Ejemplo de Gráfico Interactivo en R
```r
library(plotly)
df <- read.csv('data/processed/piura_pbi.csv')
fig <- plot_ly(df, x = ~Año, y = ~PBI, type = 'scatter', mode = 'lines+markers')
fig  # Muestra el gráfico interactivo
```
# 📚 Referencias
- INEI: https://m.inei.gob.pe/estadisticas/indice-tematico/
- Datos abiertos del Gobierno Peruano
- BCRP: Estadísticas económicas regionales
# � Métodología Científica

### Extracción de Datos
```python
# Ejemplo de código usado
import pandas as pd
from matplotlib import pyplot as plt

df = pd.read_csv('data/piura_pbi.csv')
df['Año'] = pd.to_datetime(df['Año'], format='%Y')
plt.figure(figsize=(12, 6))
plt.plot(df['Año'], df['PBI'], marker='o', linewidth=2)
plt.title('Evolución del PBI de Piura 2007-2023')
plt.savefig('visualizations/pbi_evolution.png')
```
# �🔍 Hallazgos Principales
- Crecimiento sostenido del PBI 2007-2014
- Impacto del Fenómeno del Niño Costero (2017)
- Resiliencia post-pandemia (2021-2023)
- Transformación del régimen tributario

# 👥 Autores
- Eva Colan Huaranga
- Giancarlo Gonzales Berrios  
- Gaston Diaz Guerrero

# 📄 Licencia
Este proyecto está bajo la Licencia MIT.
## 🧪 Ejemplo de Análisis en R

```r
library(ggplot2)
library(dplyr)

# Carga de datos
df <- read.csv('data/processed/piura_pbi.csv')

# Gráfico de evolución del PBI
ggplot(df, aes(x = Año, y = PBI)) +
	geom_line(color = '#2E86AB', size = 1.2) +
	geom_point(color = '#2E86AB', size = 2) +
	labs(title = 'Evolución del PBI de Piura (2007-2023)',
			 x = 'Año',
			 y = 'PBI (millones de soles)') +
	theme_minimal()
ggsave('visualizations/png/pbi_evolution_r.png', dpi = 300)
```
## 🧪 Ejemplo de Análisis en Python

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Carga de datos
df = pd.read_csv('data/processed/piura_pbi.csv')

# Gráfico de evolución del PBI
plt.figure(figsize=(12, 6))
plt.plot(df['Año'], df['PBI'], marker='o', linewidth=2, color='#2E86AB')
plt.title('Evolución del PBI de Piura (2007-2023)', fontsize=16)
plt.xlabel('Año')
plt.ylabel('PBI (millones de soles)')
plt.grid(True, alpha=0.3)
plt.savefig('visualizations/png/pbi_evolution.png', dpi=300)
plt.show()
```
## ⚙️ Instalación de Dependencias

### Python
```bash
pip install pandas matplotlib seaborn plotly numpy
```

### R
```r
install.packages(c("ggplot2", "dplyr", "tidyr", "plotly"))
```
# 📊 Análisis Socioeconómico de Piura (2007-2023)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![R](https://img.shields.io/badge/R-4.0%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📖 Descripción
Análisis integral de 15 indicadores socioeconómicos del departamento de Piura mediante visualizaciones en Python y R para la formulación de políticas públicas y toma de decisiones.

## 🎯 Objetivos

### Objetivo General
Generar un estudio que sirva de guía para la formulación de políticas públicas mediante el análisis del progreso, fluctuaciones y trayectoria de los principales indicadores socioeconómicos de Piura.

### Objetivos Específicos
- Recopilar y esquematizar información oficial del INEI
- Visualizar la trayectoria de cada indicador (2007-2023)
- Identificar etapas de auge, estancamiento o declive
- Elaborar un análisis sintético de los descubrimientos

## 📈 Variables Analizadas

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

## 🛠️ Tecnologías Utilizadas

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
```