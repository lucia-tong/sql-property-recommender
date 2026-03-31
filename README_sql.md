# SQL Property Recommender

Sistema de recomendación de alojamientos usando SQL y Python. A partir de los requisitos de un cliente real, se construye una base de datos relacional y se ejecutan queries progresivas hasta encontrar las propiedades que cumplen todos los filtros. Proyecto del Máster en Data & AI — Nuclio Digital School.

## qué hace

* convierte archivos Excel a CSV y los carga en una base de datos MySQL
* crea 4 tablas relacionales: alojamiento, ubicación, precio y puntuación
* construye queries individuales para cada requisito del cliente
* combina todos los filtros en una única query final con JOINs
* devuelve las propiedades que cumplen todas las condiciones simultáneamente

## requisitos del cliente que se modelan

* terraza y aire acondicionado, sin piscina
* no estudios sin salón, mínimo 2 baños
* superficie mínima de 80m²
* a más de 1 km del metro y 2 km del centro (cliente sensible al ruido)
* precio entre 1.500€ y 2.000€ la noche
* porcentaje de reserva exactamente del 25%
* puntuación del alojamiento > 4.5 y de la agencia > 4 puntos

## estructura

```
sql-property-recommender/
├── sql_property_recommender.ipynb   # creación de BD, queries y resultado final
└── README.md
```

## cómo ejecutarlo

```bash
pip install sqlalchemy mysql-connector-python pandas openpyxl jupyter
jupyter notebook sql_property_recommender.ipynb
```

necesitas MySQL corriendo en local. actualiza la cadena de conexión en la primera celda con tus credenciales.

## stack

python · pandas · sqlalchemy · mysql · openpyxl · jupyter
