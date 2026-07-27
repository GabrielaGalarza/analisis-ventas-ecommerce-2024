# Análisis de Ventas E-commerce 2024

Proyecto de Business Intelligence orientado al análisis del desempeño comercial de un e-commerce durante 2024.

El trabajo incluye la revisión de la calidad de los datos, su organización en Google Sheets y la creación de un dashboard interactivo en Looker Studio para visualizar indicadores relevantes sobre ventas, clientes, productos, regiones y métodos de pago.

## Problema analizado

Un comercio electrónico genera información sobre ventas, productos, clientes, regiones y medios de pago. Sin embargo, disponer de esos datos no es suficiente si no se encuentran organizados y presentados de una manera que facilite su interpretación.

Este proyecto busca transformar los registros de ventas del negocio en información útil para responder preguntas como:

- ¿Cómo evolucionaron las ventas durante el año?
- ¿Qué regiones generaron más ingresos?
- ¿Cuáles fueron los productos más vendidos?
- ¿Qué métodos de pago utilizaron los clientes?
- ¿Cuántos clientes participaron de las operaciones?
- ¿Cuál fue el ticket promedio?
- ¿La información disponible tenía la calidad necesaria para realizar el análisis?

## Objetivo

Desarrollar una solución de Business Intelligence que permita analizar el rendimiento comercial del e-commerce y facilitar la toma de decisiones basada en datos.

## Proceso de trabajo

### 1. Evaluación de la calidad de los datos

Antes de construir el dashboard se realizó una revisión del conjunto de datos considerando:

- Precisión
- Completitud
- Consistencia
- Actualidad
- Validez
- Accesibilidad
- Relevancia

No se identificaron valores vacíos ni registros duplicados. Sin embargo, se encontraron algunas inconsistencias en el formato de las fechas y falta de claridad en la codificación del campo correspondiente al método de pago.

Como mejoras se propuso:

- Estandarizar las fechas con el formato `DD/MM/AAAA`.
- Documentar los valores utilizados en el campo de método de pago.
- Definir reglas de actualización y permisos de acceso.
- Mantener la estructura general del dataset, ya que cumplía con los criterios de completitud y relevancia.

### 2. Preparación de la información

Los datos fueron organizados y revisados en Google Sheets para asegurar que tuvieran una estructura adecuada antes de conectarlos con Looker Studio.

### 3. Diseño del dashboard

Se desarrolló un dashboard interactivo con filtros por:

- Mes
- Método de pago
- Categoría
- Región

El dashboard fue dividido en dos vistas para evitar la sobrecarga de información y facilitar la lectura de los resultados.

## Indicadores principales

El dashboard presenta los siguientes KPI:

- Ventas totales
- Ticket promedio
- Clientes activos
- Ventas por región
- Evolución mensual de ventas
- Ventas por método de pago
- Productos más vendidos
- Distribución regional de las operaciones

## Principales resultados

De acuerdo con el dashboard:

- Las ventas totales alcanzaron los `$103.103,19`.
- Se registraron `326 clientes activos`.
- Las ventas tuvieron un crecimiento importante durante los primeros meses.
- El punto más alto del año se produjo en junio.
- Después de junio, las ventas se mantuvieron relativamente estables.
- Buenos Aires fue la región con mayor volumen de ventas.
- Mercado Pago fue el método de pago con mayor participación.
- Entre los productos con mayor cantidad de unidades vendidas se encontraron las hamburguesas congeladas, el agua mineral, la cerveza, la pizza congelada y las galletitas de chocolate.

## Decisiones de visualización

Durante el desarrollo también se analizaron diferentes formas de presentar los datos.

Se identificaron problemas frecuentes como:

- Exceso de métricas dentro de un mismo gráfico.
- Uso de colores con poco contraste.
- Gráficos circulares con demasiadas categorías.
- Títulos poco descriptivos.
- Mezcla de valores con escalas muy diferentes.

Para mejorar la interpretación se priorizaron:

- Gráficos de barras para comparar categorías.
- Títulos descriptivos.
- Colores consistentes.
- Separación de indicadores con escalas diferentes.
- Ordenamiento de categorías de mayor a menor.
- Distribución de la información en distintas páginas.

## Herramientas utilizadas

- Looker Studio
- Google Sheets
- Excel
- Business Intelligence
- Limpieza y validación de datos
- Diseño de dashboards
- Análisis exploratorio de datos

## Dashboard interactivo

[Ver dashboard en Looker Studio](https://datastudio.google.com/reporting/bf56af6c-31fd-44c8-97d1-bc3e69253dd9)

> El enlace se encuentra configurado únicamente para visualización.

## Vista previa

### Página 1: resumen de ventas

![Resumen del dashboard](<img width="928" height="654" alt="image" src="https://github.com/user-attachments/assets/28a80b9c-a55c-4a2f-ba36-6ea226af091f" />
)

### Página 2: productos y regiones

![Productos y regiones](<img width="926" height="654" alt="image" src="https://github.com/user-attachments/assets/fa45ef19-35d3-44a0-a01a-7066154e6ff9" />
)

## Estructura del repositorio

```text
analisis-ventas-ecommerce-2024/
│
├── README.md
├── imagenes/
│   ├── dashboard-resumen.png
│   └── dashboard-productos-regiones.png
│
├── documentos/
│   ├── analisis-calidad-datos.pdf
│   ├── proyecto-final.pdf
│   └── analisis-visualizaciones.pdf
│
└── datos/
    └── dataset-ventas-2024.csv
