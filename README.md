# TF-Fundamentos-de-Data-Science

## Objetivo del proyecto
Aplicar la metodología CRISP-DM sobre el dataset `bike_buyers` para identificar los factores que caracterizan a los clientes que compran bicicletas y construir un scoring que priorice oportunidades comerciales para la empresa Peru_bike.

## Integrantes del equipo
- Business Project Sponsor: Fabrizio Bussalleu
- Data Scientist: Facundo Maco
- Data Engineer: Renzo Arbulu
- Data Analyst: Aldo Zavala

## Conjunto de datos
- **Fuente:** `data/bike_buyers.csv` (dataset original proporcionado por la consultora).
- **Versión limpia:** `data/bike_buyers_clean.csv`, generado durante la fase de preparación para garantizar consistencia y ausencia de valores nulos.
- **Descripción general:** 1 000 registros con información sociodemográfica, financiera y de comportamiento de clientes, incluyendo la variable objetivo `Purchased Bike`.

## Estructura del repositorio
- `code/code.ipynb`: notebook principal que documenta cada fase de CRISP-DM.
- `data/bike_buyers.csv`: dataset original.
- `data/bike_buyers_clean.csv`: dataset tratado listo para modelar.
- `README.md`: guía rápida del proyecto y requisitos de entrega.

## Metodología CRISP-DM en el notebook
1. **Comprensión del negocio:** contextualiza el objetivo de Peru_bike y las preguntas analíticas.
2. **Comprensión de los datos:** inspección estructural, perfilamiento y verificación de calidad (nulos, duplicados, outliers).
3. **Preparación de los datos:** limpieza, creación de variables derivadas (`Con_hijos`, `Con_vehiculo`) y versionado del dataset limpio.
4. **Modelado:** entrenamiento de regresión logística para generar un scoring de compra.
5. **Conclusiones preliminares:** principales hallazgos para sustentar decisiones.

## Instrucciones de ejecución
1. Crear un entorno virtual (opcional) e instalar dependencias ejecutando la celda 1 del notebook (`%pip install ...`).
2. Ejecutar el notebook `code/code.ipynb` en orden secuencial para replicar la limpieza, análisis y modelado.
3. Revisar los archivos generados en `data/` para incluirlos en el informe PDF final.

## Conclusiones a destacar
- Los ingresos, la propiedad de vivienda y las variables derivadas apoyan la segmentación comercial.
- El scoring preliminar permite priorizar clientes con mayor probabilidad de compra.
- Se recomienda validar los umbrales del modelo con el equipo de negocio antes de desplegar.
