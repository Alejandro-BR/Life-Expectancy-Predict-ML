# 📄 Life_Expectancy_Data.csv

## Obtención de datos

**Fuente:** [Life Expectancy (WHO)](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)

El estudio analiza los factores que afectan la esperanza de vida en **193 países** entre **2000** y **2015**, considerando variables de salud, mortalidad, economía, sociedad e inmunización.

Los datos provienen del **Global Health Observatory** (OMS) y de **Naciones Unidas**, obtenidos de encuestas y registros oficiales. 

## Descripción de los datos

El dataset cuenta con **22 columnas** y **2928 filas**, de las cuales 2 son de tipo `object`, 4 de tipo `int64` y 16 de tipo `float64`.

El **target** que se busca predecir es **Life expectancy**, es decir, la esperanza de vida de la población en cada país y año.

| Categoría | Columnas | Tipo de dato |Descripción |
| :----- | :----- | :----- | :----- |
| Información general del país | Country | object | Nombre del país. |
| Información general del país | Year | int64 | Año de la observación. |
| Información general del país | Status | object | Estado de desarrollo del país (Desarrollado/En desarrollo). |
| Esperanza de vida | Life expectancy | float64 | Esperanza de vida promedio al nacer en años. |
| Mortalidad | Adult Mortality | float64 | Tasa de mortalidad de adultos. |
| Mortalidad | infant deaths | int64 | Número de muertes infantiles. |
| Mortalidad | under-five deaths  | int64 | Número de muertes de niños menores de 5 años. |
| Consumo de sustancias | Alcohol | float64 | Consumo de alcohol per cápita. |
| Gasto en salud | percentage expenditure | float64 | Porcentaje del gasto en salud respecto al PIB. |
| Inmunización | Hepatitis B | float64 | Porcentaje de cobertura de vacunación contra Hepatitis B. |
| Inmunización | Measles | int64 | Número de casos de sarampión. |
| Factores de salud | BMI | float64 | Índice de masa corporal promedio. |
| Inmunización | Polio | float64 | Porcentaje de cobertura de vacunación contra Polio. |
| Gasto en salud | Total expenditure | float64 | Gasto total en salud per cápita. |
| Inmunización | Diphtheria | float64 | Porcentaje de cobertura de vacunación contra Difteria. |
| Enfermedades | HIV/AIDS | float64 | Prevalencia de VIH/SIDA. |
| Economía | GDP | float64 | Producto Interno Bruto per cápita. |
| Demografía | Population | float64 | Población total del país. |
| Nutrición | thinness 1-19 years | float64 | Porcentaje de delgadez en niños de 1 a 19 años. |
| Nutrición | thinness 5-9 years | float64  | Porcentaje de delgadez en niños de 5 a 9 años. |
| Economía | Income composition of resources | float64 | Composición del ingreso de los recursos del país. |
| Educación | Schooling | float64 | Años promedio de escolaridad. |


---


```python
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 2938 entries, 0 to 2937
Data columns (total 22 columns):
 #   Column                           Non-Null Count  Dtype  
---  ------                           --------------  -----  
 0   Country                          2938 non-null   object 
 1   Year                             2938 non-null   int64  
 2   Status                           2938 non-null   object 
 3   Life expectancy                  2928 non-null   float64
 4   Adult Mortality                  2928 non-null   float64
 5   infant deaths                    2938 non-null   int64  
 6   Alcohol                          2744 non-null   float64
 7   percentage expenditure           2938 non-null   float64
 8   Hepatitis B                      2385 non-null   float64
 9   Measles                          2938 non-null   int64  
 10   BMI                             2904 non-null   float64
 11  under-five deaths                2938 non-null   int64  
 12  Polio                            2919 non-null   float64
 13  Total expenditure                2712 non-null   float64
 14  Diphtheria                       2919 non-null   float64
 15   HIV/AIDS                        2938 non-null   float64
 16  GDP                              2490 non-null   float64
 17  Population                       2286 non-null   float64
 18   thinness  1-19 years            2904 non-null   float64
 19   thinness 5-9 years              2904 non-null   float64
 20  Income composition of resources  2771 non-null   float64
 21  Schooling                        2775 non-null   float64
dtypes: float64(16), int64(4), object(2)
memory usage: 505.1+ KB
```