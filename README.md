
# <h1 align=center> **PI ANÁLISIS DE CRIPTOMONEDAS CON API COINGECKO** </h1>
## **_By: Leydy Lucena Peñaloza Rojas_**
<img src="Imagenes/Autora_Leydy_Penaloza.png" alt="Autora" width="150"/>


# Proyecto de Análisis de Criptomonedas

## Introducción

Este repositorio contiene un proyecto de análisis de datos sobre las principales criptomonedas utilizando la API pública de Coingecko y Binance.

En este proyecto se muestra un análisis de las criptomonedas en el ranking de las 10 primeras en cuanto a capitalización de mercado.


## Objetivo
El objetivo principal de este proyecto es realizar un Análisis Exploratorio de Datos (EDA) en las criptomonedas más destacadas del mercado para obtener información valiosa sobre sus precios, tendencias y comportamientos.

## Fuentes de Datos
- Se extrajo información de la API Pública de Coingecko para obtener datos sobre las criptomonedas.
- Se extrajo información de la API pública de Binance para obtener datos de precio de apertura, máximo, mínimo, cierre y volumen

## ETL y Datos Históricos
- Para el presente proyecto se tomará como referencia las `10 primeras criptomonedas` ubicadas en el ranking de market cap para ello se generó el dataset `Top_10_Criptomonedas.csv` que contiene la información básica de las 10 criptomonedas seleccionadas.

- Se realizó un segundo ETL para obtener los valores históricos de los últimos 10 años de las criptomonedas seleccionadas, con los datos de periodicidad diaria, incluyendo precio de cierre, capitalización de mercado y volumen y se guardaron en el dataset `historical_prices.csv`.

- Se intentó obtener información OHLCV, pero al no ser posible con la API Coingecko, se utilizó la API pública de Binance para obtener datos de apertura, máximo, mínimo, cierre y volumen. Se generó el dataset `OHLCV_data.csv`.

## Análisis Exploratorio de Datos (EDA)
Se llevaron a cabo varios análisis en el EDA:

1. **Distribución de precios:** Se exploró la distribución de los precios de las criptomonedas para identificar rangos comunes, valores atípicos y tendencias generales.

2. **Relación entre capitalización de mercado y precio:** Se analizó cómo se relacionan la capitalización de mercado y el precio de cada criptomoneda para identificar discrepancias potenciales.

3. **Tendencias alcistas o bajistas:** Se observaron las tendencias generales de aumento o disminución en los precios a lo largo del tiempo.

4. **Análisis de Volumen de Negociación:** Se examinó el volumen de negociación diario para entender el interés y la liquidez en el mercado.

## Resultados y Conclusiones
- Se identificaron patrones de comportamiento similar en las criptomonedas seleccionadas, incluyendo un pico en el precio entre noviembre de 2020 y noviembre de 2021, seguido de una disminución en los precios en los años siguientes.
- La resistencia histórica de los precios en comparación con los valores de noviembre de 2020 sugiere una estabilidad relativa.
- El proyecto resalta la importancia de considerar factores macroeconómicos y eventos del mercado en el análisis de criptomonedas.

## Imágenes
![Gráfico de Precios](/Imagenes/Grafico_precios1.JPG)
![Gráfico de Relación](/Imagenes/Grafico_precios2.JPG)
![Gráfico de Tendencias](/Imagenes/Grafico_precios3.JPG)
![Gráfico de Volumen](/Imagenes/Grafico_precios4.JPG)