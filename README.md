![](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/suelos_peru.png)

# Análisis de muestreos geoquímicos de suelos superficiales usando métodos no supervisados de aprendizaje automático como estrategia para la prospección de yacimientos minerales en Perú.

### Integrantes: 

**Diana Urbano**

**Edinson Fernandez**

**Daren Rodríguez**

# Resumen

Entre el año 2000 al 2019 se realizaron diversos muestreos geoquímicos por el Instituto Geológico, Minero y Metalúrgico de Perú, de los cuales se tomó una base de datos con 536 muestras de suelos superficiales para la prospección de yacimientos minerales.
En este análisis se usaron técnicas de aprendizaje automático no supervisado hallando 9 componentes principales que explican el 80% de la varianza y usando el clúster aglomerativo con mejores agrupaciones que el DBSCAN, hallando 13 clústeres de los cuales 4 tienen correlaciones significativas con elementos indicadores de yacimientos minerales, con el clúster 6 indicando la presencia de un yacimiento, asociado a Au, Ag, Hg, Bi mientras que los otros 2 clústeres (8 y 10) se asocian con elementos de interés como: Au, Ag, Cu, Zn, Pb, In entre otros, y en menor medida el clúster 9 se asocia con Mo,V,Ni,Tl indicando yacimientos posiblemente hidrotermales o se sulfuros masivos. Estas agrupaciones delimitan nuevas zonas de prospección minera de 50 km entre la zona de Huancayo y Jauja siguiendo la rivera del rio Mantaro y otra zona puntual cerca a Cochamarca. Para estas dos zonas se recomienda realizar un mapeo geológico más detallado y decidir si se realizan estudios especializados.

# Base de datos original

La información se encuentra disponible para libre descarga por el Instituto Geológico, Minero y Metalúrgico de Perú en su plataforma GEOCATMIN y pertenecen a la serie B Prospección Geoquímica del Perú.
El archivo 2_BD_Geoquímica de Suelos.rar corresponde a 4 documentos de Excel con muestras de suelo superficial y suelo profundo en Perú. Para los fines de este trabajo se unificaron los Excel de suelos superficiales en un solo documento y usando solamente la información del laboratorio INGEMMET.
Enlaces de descarga: 
https://www.gob.pe/institucion/ingemmet/informes-publicaciones/1423546-base-de-datos-de-geoquimica

* [Archivos base de datos original](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/Bases%20de%20datos/2_BD_Geoqu%C3%ADmica%20de%20Suelos.rar.rar)

# Base de datos luego del proceso de limpieza

La base de datos unificada de suelos superficiales contiene inicialmente 540 registros que posteriormente luego de la limpieza se reducen a 536 registros de muestras.

![imagen](https://user-images.githubusercontent.com/92902914/192127813-ba3f33d1-f085-4a5c-ab98-9e6642bc77b8.png)

* [Base de datos con limpieza de datos(Excel)](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/Bases%20de%20datos/Base_suelos_limpia.xlsx)

# 9 componentes principales 

![imagen](https://user-images.githubusercontent.com/92902914/192127369-a748780b-5631-4f2a-88ea-0c1fbbc78021.png)

# Dendograma

![imagen](https://user-images.githubusercontent.com/92902914/192127386-b433b746-4318-47e2-b25c-738cb6007338.png)


# 13 cluster con el metodo aglomerativo

![imagen](https://user-images.githubusercontent.com/92902914/192127592-8be93915-41b7-4837-972e-245fe231c7ec.png)


# Correlación de los 13 cluster con los elementos y oxidos

![imagen](https://user-images.githubusercontent.com/92902914/192127328-a6f49425-4376-42fb-8073-9f05f3d87985.png)

![imagen](https://user-images.githubusercontent.com/92902914/192127643-16b740fc-1b3b-457a-90b8-a828bb1b6f6c.png)


# Mapa web con las 536 muestras geoquímicas de suelos

[Mapa web 536 muestras](https://djrodriguezc1.github.io/Mapa-geoquimico-suelos-Per-/)

# Mapa con todos los cluster

![pathfinders_Total](https://user-images.githubusercontent.com/92902914/192126964-e519b518-fa13-4e46-86a5-ac420be1f990.png)


# Mapa con los cluster principales

![pathfinders_6_8_9_10](https://user-images.githubusercontent.com/92902914/192127060-ea9b3926-f0b7-49a0-8e5d-db3db8ededca.png)

# Codigo

[Codigo](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/Codigo/suelos_p.ipynb)

# Correlación entre cluster y variables

[Excel correlación entre cluster aglomerativo y variables]()

# Grafica plotly con los cluster aglomerativo 

[Grafica 3d cluster aglomerativo](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/Graficas%203d%20cluster/agglom13.html)


# Base de datos con los cluster finales

[Base de datos cluster](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/Base%20de%20datos%20final/base_clusters13_n.xlsx)

# Informe final

[Informe Final (pdf)](https://github.com/djrodriguezc1/Analisis-geoquimico-de-suelos-usando-metodos-no-supervisados/blob/main/Informe%20Final/Informe_final_grupo_8.pdf
)
