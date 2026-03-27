# Estudio de embudos en el proceso de compra
![Static Badge](https://img.shields.io/badge/-Python-%233776AB?logo=python&logoColor=white)

## Descripción del proyecto 
Proyecto desarrollado para una hipotética empresa de venta de entradas a eventos.

## Objetivo del proyecto
El objetivo es optimizar los gastos de marketing. Para ello nos interesa detectar:
* Cómo los clientes usan el servicio
* Cuando empiezan a comprar
* Cuánto dinero aporta cada cliente a la compañía
* Cuando los ingresos cubren el costo de adquisición de los clientes

## Metodología
1. Cargar dataset
2. Data Cleaning (Preparación): Remover errores, inconsistencias, duplicados, procesar datos faltantes y unir varias tablas.
3. Análisis exploratorio de los datos (EDA): Realizar un análisis preliminar del comportamiento de los usuarios en cada etapa del embudo de compra.
4. Modelado de datos e interpretación: Aplicar pruebas estadísticas (SciPy) para extraer información útil.
5. Visualización (Matplotlib) y reportar

## Descripción de los datos:

Tabla ‘visits’: Registros del servidor con datos sobre las visitas al sitio web:
* Uid: identificador único del usuario
* Device: dispositivo del usuario
* Start Ts: fecha y hora del inicio de sesion
* End Ts: fecha y hora de término de la sesion
* Source Id: identificador de la fuente de anuncios de la que proviene el usuario.

Tabla ‘orders’: Datos sobre los pedidos:
* Uid: identificador único del usuario que realiza un pedido
* Buy Ts: fecha y hora del pedido
* Revenue: el ingreso de la empresa por el pedido

Tabla ‘costs’: Datos sobre gastos de marketing
* source_id: identificador de la fuente de anuncios
* dt: fecha
* costs: gastos en esta fuente de anuncio en este dia
