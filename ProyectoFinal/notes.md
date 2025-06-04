# Notes 

Geospatial data that support health research can be categorized into four broad types, as follows.  
(i) Data about healthcare capacities, such as health facilities, employment, and administration.  
(ii) Data about the population and their health conditions and healthcare needs. The demographic health survey data, which are surveyed in many countries describing disease outbreak rates and other health indicators of the population, are often published with map coordinates of surveyed clusters.  
(iii) Data about the environment, both natural and social, which affects people's health. For example, the long standing water may affect the dispersion of malaria, which in turn affects the surrounding resident's health.
(iv) Data about transportation and the address location of patients is essential in understanding the accessibility for care, dissemination of medical supply, traffic routing, connectivity among street/road segments, transmission of infectious diseases, distribution of patients, best route and travel time, and locating a place with its postal address or longitude and latitude coordinates.

- Prevalencia
- Insidencia
- Mortalidad
- Densidad Poblacional
- Disponibilidad y accesibilidad a centros de salud
- Caracteristicas ambientales (Temperatura, Humedad, Altura MSNM. Pluviosidad)


Variables dependientes
- Tasa de letalidad =  No. Muertes/No.muertes+No.Recuperados x 100

Environment Factors
- average elevation
- average annual rainfall
- avarage annual temperature
- area km2
- population


Variables geograficas:





my_data_covid19
----------------

codigo_subregion
nombre_subregion
codigo_municipio
nombre_municipio
area
poblacion
densidad
precipitacion
temperatura
altitud
fecha_reporte
muertes_covid19
recuperados_covid19
geometry (POINTS)


poblacion_mpios_antioquia
-------------------------
codigo_municipio
nombre_municipio
?? >> codigo_subregion
nombre_subregion
poblacion
hombres
mujeres

geo_mpios_antioquia
--------------------
mpio_cdpmp  >> codigo_municipio
mpio_cnmbr >> nombre_municipio  
mpio_narea  >> area_municipio
shape_Leng  
shape_Area
geometry  (Polygon)

geo_subregiones_antioquia 
------------------------
COD_SUBREG  >> codigo_subregion  
SUBREGION >> nombre_subregion
geometry (Polygon)

meteorologia_mpios_antioquia
----------------------------
codigo_municipio
nombre_municipio
precipitacion
temperatura
altitud

add geodataframe & dataframe

# Merge with `merge` method on shared variable (iso codes):
country_shapes = country_shapes.merge(country_names, on='iso_a3')

Clean 
Estandarizacion de los nombres de variables y valores