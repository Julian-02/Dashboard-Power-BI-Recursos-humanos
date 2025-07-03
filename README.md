# Dashboard | Power Bi | Recursos-humanos
Dasboard de gastos en Recursos humanos Power Bi - Base de datos Excel o SQL server 

Link exposición del proyecto: https://youtu.be/fFlpSgnGQnM

Este repositorio contiene un dashboard interactivo desarrollado en **Power BI** para el análisis detallado de **gastos presupuestales en el área de Recursos Humanos (RR.HH.)**. 

El tablero fue diseñado desde una perspectiva técnica de **ciencia de datos**, e incluye el modelado de datos, métricas calculadas con DAX, visualizaciones estratégicas y recomendaciones basadas en análisis descriptivo y prescriptivo.

---

## 📌 Objetivo

Proporcionar a analistas, científicos de datos y líderes de RR.HH. una herramienta para:
- Visualizar la ejecución presupuestal.
- Detectar sobrecostos o subejecuciones por categoría.
- Analizar el comportamiento del gasto en el tiempo.
- Tomar decisiones informadas basadas en datos.

---

## 📊 Estructura del Dashboard

El tablero incluye las siguientes secciones visuales:

| Visualización                       | Métrica principal                 | Objetivo                                                  |
|------------------------------------|----------------------------------|-----------------------------------------------------------|
| Indicadores clave (cards & gauges) | Total Gastado, % Ejecutado, Saldo| Evaluar el estado general del presupuesto                |
| Barras horizontales                | Gastos por Categoría             | Identificar rubros más costosos (Análisis ABC)           |
| Líneas                             | Gasto por Mes                    | Detectar estacionalidades o comportamientos atípicos     |
| Columnas por Trimestre             | Acumulado Trimestral             | Evaluar evolución inter-trimestral del gasto             |
| Dona                               | Gasto por Semestre               | Detectar concentraciones semestrales                     |
| Tabla Detallada                    | KPIs por Categoría               | Comparación granular con % ejecución y saldos            |


![image](https://github.com/user-attachments/assets/fe034150-8a3c-4aa7-9963-05bffb2896dc)

---

## 🧠 Técnicas de Ciencia de Datos Aplicadas

### 🔹 Modelado Estrella (Star Schema)
- `Gastos1` (tabla de hechos) conectada a `Presupuesto2` y `Calendario`.

### 🔹 Métricas en DAX
- `Total Gastado`, `Saldo`, `% de Ejecución`, entre otros, usando funciones `SUM`, `DIVIDE`, `CALCULATE`, etc.

### 🔹 Análisis Descriptivo
- Estado actual del presupuesto y desglose por categorías.

### 🔹 Análisis Temporal
- Evolución mensual, trimestral y semestral usando jerarquías de fechas.

### 🔹 Análisis Comparativo
- Benchmark entre presupuesto asignado y gasto ejecutado por categoría.

### 🔹 Visual Analytics
- Uso de gráficos interactivos y condicionales para storytelling con datos.

### 🔹 Principio de Pareto (80/20)
- Identificación de rubros que consumen mayor proporción del gasto.

---

## 📁 Estructura del Repositorio

📦RRHH-Gastos-Dashboard
┣ 📁assets
┃ ┣ 📸 screenshot_dashboard.png
┃ ┗ 📸 thumbnail_video.png
┣ 📄 Gastos_RRHH.pbix
┣ 📄 README.md
┗ 📄 LICENSE

yaml
Copiar
Editar

---

## 🛠️ Requisitos

- Power BI Desktop (versión reciente)
- Fuente de datos estructurada (Excel, SQL Server, etc.)
- Conexión correcta entre tablas:
  - `Gastos1[Fecha]` → `Calendario[Fecha]`
  - `Gastos1[Categoría]` → `Presupuesto2[Categoría]`

