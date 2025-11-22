# 🏙️ **Life Expectancy Predict ML**

El proyecto trata de construir un modelo de Machine Learning capaz de **predecir la esperanza de vida en un país determinado** a partir de distintos factores relacionados con la salud, la economía y la demografía.

## Obtención de datos

**Fuente del dataset original:** [Life Expectancy (WHO)](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)

**Dataset:** [Life_Expectancy_Data.csv](/data/raw/Life_Expectancy_Data.csv)

El estudio analiza los factores que afectan la esperanza de vida en **193 países** entre **2000** y **2015**, considerando variables de salud, mortalidad, economía, sociedad e inmunización.

Los datos provienen del **Global Health Observatory** (OMS) y de **Naciones Unidas**, obtenidos de encuestas y registros oficiales.

![Life expectancy](/img/life_expectancy.png)

## Modelo de machine learning

El **target** que se busca predecir es **life_expectancy**, es decir, la esperanza de vida de la población en cada país y año.

**Modelo:** [RandomForestRegressor](/models/rf_model.joblib)

* R² = 0.969
* RMSE = 1.648
* MAPE = 1.53%

**Dataset limpio:** [life_expectancy_data.csv](/data/processed/life_expectancy_data.csv)

El dataset cuenta con 204 columnas y 2928 filas, de las cuales:

| Categoría | Columnas | Tipo de dato | Descripción |
| :----- | :----- | :----- | :----- |
| Información general del país | year | int64 | Año de la observación. |
| Información general del país | is_developed | int64 | Variable binaria que indica si el país está desarrollado (1) o en desarrollo (0). |
| Esperanza de vida | life_expectancy | float64 | Esperanza de vida promedio al nacer en años. |
| Mortalidad | adult_mortality | float64 | Tasa de mortalidad de adultos. |
| Mortalidad | infant_deaths | int64 | Número de muertes infantiles. |
| Mortalidad | under_five_deaths | int64 | Número de muertes de niños menores de 5 años. |
| Consumo de sustancias | alcohol | float64 | Consumo de alcohol per cápita. |
| Gasto en salud | percentage_expenditure | float64 | Porcentaje del gasto en salud respecto al PIB. |
| Inmunización | hepatitis_b | float64 | Porcentaje de cobertura de vacunación contra Hepatitis B. |
| Inmunización | measles | int64 | Número de casos de sarampión. |
| Factores de salud | bmi | float64 | Índice de masa corporal promedio. |
| Inmunización | polio | float64 | Porcentaje de cobertura de vacunación contra Polio. |
| Gasto en salud | total_expenditure | float64 | Gasto total en salud per cápita. |
| Inmunización | diphtheria | float64 | Porcentaje de cobertura de vacunación contra Difteria. |
| Enfermedades | hiv_aids | float64 | Prevalencia de VIH/SIDA. |
| Economía | gdp | float64 | Producto Interno Bruto per cápita. |
| Demografía | population | float64 | Población total del país. |
| Nutrición | thinness_1_19_years | float64 | Porcentaje de delgadez en niños de 1 a 19 años. |
| Nutrición | thinness_5_9_years | float64 | Porcentaje de delgadez en niños de 5 a 9 años. |
| Economía | income_composition_of_resources | float64 | Composición del ingreso de los recursos del país. |
| Educación | schooling | float64 | Años promedio de escolaridad. |
| Información general del país | country_spain, country_italy, …, | int64 | Variables binarias (0/1) que indican a cada país. |

## Google Colab

[Cuaderno jupyter](https://colab.research.google.com/drive/16Eevl7m9phEPlVpiEsviADw3Nn0YhStA?usp=sharing)

## Creditos:

Práctica: **[Índice de proyectos de todos los alumnos](https://github.com/CPIFPAlanTuring/iabd-proyecto-ml-2526)**

Máster de FP en Inteligencia Artifical y Big Data - CPIFP Alan Turing