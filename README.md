# Análisis de registros clínicos simulados

**Estudiante:** Gina Valentina Gómez Rivadeneira  
**Proyecto:** Análisis de registros clínicos simulados  
**Herramienta utilizada:** Microsoft Excel  
**Tipo de datos:** Registros clínicos simulados con fines académicos  

## 1. Objetivo del proyecto

Organizar y analizar una base de registros clínicos simulados mediante Microsoft Excel para calcular e interpretar siete indicadores descriptivos, reconocer datos faltantes e inconsistencias de formato y reflexionar sobre la importancia de la privacidad clínica.

El análisis es académico y descriptivo. No pretende establecer diagnósticos ni reemplazar la valoración de profesionales de la salud.

## 2. Diccionario de datos

La hoja de cálculo contiene 20 registros, identificados mediante un código. Las variables utilizadas son:

| Campo | Descripción | Tipo de dato / formato |
|---|---|---|
| `código` | Identificador único asignado a cada registro (P001–P020). | Texto |
| `Edad` | Edad consignada para el paciente. | Numérico, años |
| `Sexo` | Categoría registrada en la base (F o M). | Categórico |
| `Fecha de consulta` | Fecha asociada a la consulta. | Fecha |
| `Motivo` | Motivo de consulta registrado. | Texto |
| `temperatura (°C)` | Temperatura consignada para el registro. | Numérico, grados Celsius |
| `frecuencia cardíaca (lpm)` | Frecuencia cardíaca registrada. | Numérico, latidos por minuto |
| `saturación de oxígeno (%)` | Saturación de oxígeno. En la hoja original los valores están expresados como fracciones decimales (por ejemplo, 0,91 equivale a 91 %). | Numérico; escala decimal en el archivo original |
| `diagnóstico simulado` | Etiqueta diagnóstica ficticia incluida con fines académicos. | Texto |
| `estado de atención` | Estado registrado: Finalizada, En atención o Pendiente. | Categórico |

Las filas de resumen y gráficos que aparecen después de los 20 registros no corresponden a pacientes y no forman parte del conjunto de observaciones.

## 3. Proceso de revisión y limpieza

Para preparar e interpretar la información se siguieron estos criterios:

1. **Identificación del rango de datos:** se consideraron únicamente las 20 filas correspondientes a los códigos P001–P020. Se excluyeron del análisis las filas posteriores que contienen títulos, indicadores y datos auxiliares para gráficos.
2. **Revisión de campos:** se identificaron las variables y sus tipos de datos para distinguir campos numéricos, fechas y categorías.
3. **Revisión de valores faltantes:** se detectó un valor ausente en la saturación de oxígeno del registro P016. Se conservó como faltante; no se estimó ni se reemplazó.
4. **Revisión de unidades:** se observó que la saturación está almacenada como fracción decimal, aunque el encabezado utiliza el símbolo de porcentaje. Se documentó la equivalencia para interpretar correctamente los resultados (0,91 = 91 %).
5. **Revisión de consistencia textual:** se observaron diferencias de mayúsculas y minúsculas en algunas etiquetas de diagnóstico, además de espacios no estándar en encabezados. Se señalan como aspectos que conviene normalizar antes de realizar análisis automatizados.
6. **Cálculo e interpretación:** se revisaron los siete indicadores: total de pacientes, edad promedio, temperatura promedio, distribución por sexo, estado de atención, saturación mínima y cantidad de registros sin saturación.

Los criterios anteriores describen la revisión realizada sobre la estructura del archivo. No se modificaron ni se inventaron valores clínicos para completar información ausente.

## 4. Archivos entregados

- **`Base_Datos_Hospital.xlsx`**: archivo de Excel con la base de registros clínicos simulados, los indicadores y elementos de resumen.
- **`analisis.md`**: documento con la interpretación de los siete indicadores, las inconsistencias identificadas, la reflexión sobre privacidad clínica y una conclusión.
- **`README.md`**: este documento, que presenta el objetivo, el diccionario de datos, el proceso de revisión y limpieza, los archivos entregados y la declaración sobre el origen de los datos.

## 5. Declaración de datos ficticios

La totalidad de los registros incluidos en este proyecto es **ficticia** y fue preparada exclusivamente con fines académicos. No corresponde a pacientes reales ni debe utilizarse para tomar decisiones clínicas. Los códigos, edades, fechas, motivos de consulta, mediciones y etiquetas diagnósticas forman parte de un ejercicio simulado. Por tanto, el análisis no contiene ni pretende representar información clínica real.
