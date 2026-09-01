# Dashboard Académico – Análisis de Rendimiento y Riesgo de Abandono Estudiantil

Un dashboard interactivo desarrollado en **Power BI** para analizar el rendimiento académico de estudiantes universitarios e identificar factores asociados al riesgo de abandono mediante indicadores, segmentación y visualizaciones dinámicas.

> Proyecto desarrollado con fines **didácticos**, enfocado en demostrar el proceso de transformación de datos, modelado en Power BI y creación de indicadores utilizando DAX.

---

## Vista previa del dashboard

Factores de Riesgo 

<img width="1437" height="807" alt="factores_riesgo" src="https://github.com/user-attachments/assets/a7e4976c-98f6-4e1a-91f5-877df02d0a55" />

Rendimiento Académico 

<img width="1439" height="807" alt="rendimiento" src="https://github.com/user-attachments/assets/908b7615-8ed8-448c-96cc-5049706c7c28" />

Monitoreo Académico 

<img width="1439" height="799" alt="monitoreo" src="https://github.com/user-attachments/assets/555c35b4-6a85-4a53-aea2-91f5b3ce1944" />


---

# Objetivo del proyecto

Construir un dashboard que permita explorar el desempeño académico de los estudiantes mediante indicadores interactivos, facilitando la identificación de patrones relacionados con:

* Rendimiento académico
* Asistencia
* Estrés
* Retrasos
* Riesgo de abandono
* Variables socioacadémicas como beca, género, semestre y trabajo de medio tiempo.

---

# Dataset utilizado

El dashboard utiliza un conjunto de datos académicos que contiene información sobre estudiantes y su desempeño.

### Variables principales

| Variable             | Descripción                        |
| -------------------- | ---------------------------------- |
| GPA                  | Promedio académico del estudiante  |
| Tasa_Asistencia      | Porcentaje de asistencia           |
| Dias_Retraso         | Cantidad de días de retraso        |
| Nivel_Estres         | Nivel de estrés reportado          |
| Semestre             | Semestre cursado                   |
| Departamento         | Departamento académico             |
| Genero               | Género del estudiante              |
| Nivel_Estudio        | Nivel académico                    |
| Beca                 | Indica si recibe beca              |
| Trabajo_Medio_Tiempo | Indica si trabaja mientras estudia |
| Abandono             | Estado de abandono académico       |

---

# Proceso de desarrollo

## 1. Transformación de datos (Power Query)

Antes de crear las visualizaciones se realizó un proceso de preparación de datos utilizando **Power Query**.

### Transformaciones implementadas

* Limpieza y organización de variables académicas
* Conversión de variables continuas en categorías para facilitar el análisis
* Estandarización de variables categóricas utilizadas en filtros
* Creación de variables derivadas para clasificar estudiantes según su desempeño y nivel de riesgo

### Variables creadas

| Variable creada  | Propósito                                                             |
| ---------------- | --------------------------------------------------------------------- |
| Nivel_GPA        | Clasificación del rendimiento académico (Bajo, Medio y Alto)          |
| Nivel_Asistencia | Agrupa estudiantes según porcentaje de asistencia                     |
| Grupo_Retraso    | Clasifica el número de días de retraso                                |
| Nivel_Riesgo     | Identifica estudiantes con riesgo académico según criterios definidos |

Estas transformaciones permiten construir análisis comparativos y segmentaciones dinámicas dentro del dashboard.

---

## 2. Medidas DAX implementadas

Se desarrollaron indicadores utilizando DAX para obtener métricas dinámicas.

### Indicadores principales

| Medida              | Función                                                         |
| ------------------- | --------------------------------------------------------------- |
| Total Estudiantes   | Cuenta el total de registros                                    |
| Total Desertores    | Cuenta estudiantes que abandonaron                              |
| Tasa Abandono %     | Calcula el porcentaje de abandono                               |
| GPA Promedio        | Calcula el promedio general del GPA                             |
| Asistencia Promedio | Calcula el promedio de asistencia                               |
| Estudiantes Riesgo  | Cuenta estudiantes clasificados en riesgo                       |
| Riesgo %            | Calcula el porcentaje de estudiantes en riesgo                  |
| GPA Riesgo          | Promedio del GPA para estudiantes en riesgo                     |
| KPI Abandono        | Indicador ejecutivo mostrado en tarjetas                        |
| Color Riesgo        | Medida utilizada para formato condicional                       |
| Insight Abandono    | Genera un mensaje dinámico según el comportamiento de los datos |

# Páginas del dashboard

## Factores de Riesgo

Analiza variables relacionadas con el abandono académico.

Incluye visualizaciones de:

* Distribución por nivel de riesgo.
* Nivel de estrés.
* Asistencia.
* Retrasos.
* Comparación por semestre y departamento.

**Objetivo:** identificar los principales factores asociados al riesgo de abandono.

---

## Rendimiento Académico

Explora el desempeño general de los estudiantes.

Visualizaciones principales:

* GPA promedio
* Asistencia promedio
* Comparación por género
* Comparación por beca
* Comparación por nivel de estudio

**Objetivo:** evaluar diferencias en el rendimiento entre distintos grupos de estudiantes.

---

## Monitoreo Académico

Presenta indicadores ejecutivos y seguimiento del desempeño.

KPIs incluidos:

* Total de estudiantes.
* Tasa de abandono.
* Estudiantes en riesgo.
* GPA promedio.
* Asistencia promedio.
* Insights dinámicos.

**Objetivo:** ofrecer una vista resumida para el monitoreo institucional.

---

# Interactividad del dashboard

El dashboard incorpora elementos interactivos para facilitar la exploración de la información.

### Segmentadores disponibles

* Semestre
* Departamento
* Género
* Nivel de GPA
* Nivel de riesgo

### Funcionalidades implementadas

* Cross-filtering entre gráficos
* KPIs dinámicos
* Formato condicional por nivel de riesgo
* Navegación entre páginas
* Actualización automática de indicadores según filtros seleccionados

---

# Aprendizajes obtenidos

Durante este proyecto se fortalecieron conocimientos en:

* Preparación y categorización de datos.
* Creación de indicadores académicos mediante DAX.
* Construcción de dashboards orientados al análisis educativo.
* Uso de filtros y segmentadores para análisis interactivo.
* Diseño de reportes con enfoque didáctico para cursos de análisis de datos.

---

## Autor

**Wara López**

Ingeniera Electrónica 

Este proyecto forma parte del reporsitorio de recursos didácticos y proyectos aplicados utilizando herramientas de análisis y visualización de datos.
