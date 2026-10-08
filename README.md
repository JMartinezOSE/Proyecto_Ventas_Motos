# Proyecto_Ventas_Motos
Analisis de ventas de motocicletas - Diplomado Ciencia de Datos FIME
 Análisis de Ventas de Motos
Proyecto  — Diplomado Ciencia de Datos con Python
Autor: Jose Alejandro Martinez Juarez
Instructora — Ing. Bárbara Saldaña
=Descripción
Este proyecto realiza un análisis exploratorio completo sobre un dataset de 1,500 registros de ventas de motocicletas, que incluye información de clientes, características de las motos, precios, sucursales y resultados de venta.
=Librerías Utilizadas

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

=Archivos del Proyecto
Ventas_Motos.csvDataset original con datos sucios
Proyecto_Modulo1_JoseMtz.ipynb


=Estructura del Dataset

El dataset contiene 25 columnas organizadas en 4 categorías:
Cliente: Nombre, Apellido, Edad, Sexo, Ciudad
Moto: Marca, Modelo, Tipo, Cilindraje, Color, Año, Kilometraje
Venta: Precio Lista, Descuento, Precio Final, Forma de Pago, Sucursal, Vendedor
Resultado: Estado Venta, Satisfacción, Año y Mes de Venta


=Limpieza de Datos

El dataset contenía los siguientes problemas que fueron corregidos:
40 valores nulos en columna Edad → rellenados con la mediana
40 valores nulos en columna Kilometraje → rellenados con 0
40 valores nulos en columna Satisfaccion_1_5 → rellenados con la mediana
5 outliers de edad imposible (edad = 200) → corregidos a NaN y luego a mediana
10 registros con Precio_Final = 0 → eliminados
15 registros duplicados → eliminados

= KPIs Calculados
Total de ventas concretadas
Ingreso total y precio promedio por moto
Marca más vendida y sucursal más exitosa
Forma de pago preferida por los clientes
Satisfacción promedio del cliente (escala 1-5)
Crecimiento de ingresos por año (2022-2025)

= Gráficas Generadas
Barras — Unidades vendidas por marca → identifica las marcas líderes
Línea — Crecimiento de ingresos por año → muestra tendencia de ventas
Pay — Distribución del estado de ventas → proporción vendida vs cancelada




=Cómo ejecutar el proyecto





1.-Clona el repositorio:
2.-Abre Proyecto_Motos_JoseMtz.ipynb en Jupyter Notebook
3.-Asegúrate de tener Ventas_Motos.csv en la misma carpeta
4.-Ejecuta todas las celdas con Kernel → Restart & Run All



= Conclusiones
El dataset presentaba datos sucios que fueron identificados y corregidos exitosamente.
Las ventas muestran una tendencia de crecimiento positiva entre 2022 y 2025.
La mayoría de clientes prefiere financiamiento sobre pago de contado.
La satisfacción promedio del cliente es alta, superior a 4.0/5.0.
