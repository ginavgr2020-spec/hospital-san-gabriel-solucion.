# 🏥 Hospital San Gabriel
## Informe de práctica: Análisis de registros clínicos simulados

**Estudiante:** Gina Valentina Gómez Rivadeneira  
**Proyecto:** Análisis de registros clínicos simulados  
**Herramienta utilizada:** Microsoft Excel  
**Tipo de datos:** Registros clínicos simulados con fines académicos

---

## 1. Introducción

El procesamiento de datos en el ámbito de la salud permite optimizar la toma de decisiones, identificar prioridades de atención y realizar un seguimiento estadístico eficiente de los pacientes.

En esta práctica académica se analiza un conjunto de datos compuesto por 20 registros clínicos simulados del Hospital San Gabriel. Se evalúan variables demográficas, constantes vitales y estados de atención con el propósito de aplicar herramientas de organización de datos, funciones estadísticas de Excel e interpretación clínica básica.

**Nota:** Los registros utilizados son simulados y se emplean exclusivamente con fines educativos.

## 2. Objetivos

### 2.1. Objetivo general

Analizar e interpretar un conjunto de datos de 20 registros médicos simulados mediante herramientas de organización de datos y cálculos estadísticos en Excel.

### 2.2. Objetivos específicos

- Consolidar y tabular información clínica relacionada con la edad, el sexo, la temperatura, el pulso, la saturación de oxígeno y el estado de atención.
- Aplicar funciones estadísticas de Excel, como `PROMEDIO`, `CONTAR.SI`, `MIN` y `CONTAR.BLANCO`, para obtener métricas relevantes.
- Identificar hallazgos y posibles alertas clínicas dentro del grupo de pacientes evaluados.
- Examinar la integridad de los registros para detectar datos faltantes.
- Reconocer la utilidad del análisis de datos en la organización y priorización de la atención sanitaria.

## 3. Metodología y fórmulas empleadas en Excel

Se analizaron 20 registros clínicos simulados mediante funciones estadísticas y de conteo en Excel.

Las fórmulas se aplicaron a los rangos correspondientes de la base de datos, considerando los registros comprendidos entre las filas 2 y 21.

### 3.1. Total de registros

**Fórmula:**

```excel
=CONTARA(A2:A21)
```

**Resultado:** 20 pacientes.

Esta función permite contar las celdas no vacías del rango seleccionado.

### 3.2. Promedio de edad

**Fórmula:**

```excel
=PROMEDIO(C2:C21)
```

**Resultado:** 43,0 años.

El resultado representa la edad promedio de los pacientes incluidos en el conjunto de datos.

### 3.3. Promedio de temperatura

**Fórmula:**

```excel
=PROMEDIO(F2:F21)
```

**Resultado:** 37,15 °C.

Este cálculo permite conocer la temperatura promedio registrada en el grupo analizado.

### 3.4. Distribución por sexo

**Pacientes de sexo femenino:**

```excel
=CONTAR.SI(B2:B21;"F")
```

**Resultado:** 10 pacientes (50 %).

**Pacientes de sexo masculino:**

```excel
=CONTAR.SI(B2:B21;"M")
```

**Resultado:** 10 pacientes (50 %).

La distribución muestra una representación equivalente de ambos grupos dentro de los registros analizados.

### 3.5. Estado de atención

**Consultas finalizadas:**

```excel
=CONTAR.SI(J2:J21;"*Finalizada*")
```

**Resultado:** 9 pacientes (45 %).

**Pacientes en atención:**

```excel
=CONTAR.SI(J2:J21;"En atención")
```

**Resultado:** 7 pacientes (35 %).

**Pacientes pendientes:**

```excel
=CONTAR.SI(J2:J21;"Pendiente")
```

**Resultado:** 4 pacientes (20 %).

Estos resultados permiten identificar cómo se distribuyen los registros según el estado de atención.

### 3.6. Mínima saturación de oxígeno

**Fórmula:**

```excel
=MIN(H2:H21)
```

**Resultado:** 91 %.

Este valor corresponde a la menor saturación de oxígeno registrada entre las celdas numéricas del rango analizado.

### 3.7. Calidad e integridad de los datos

**Fórmula:**

```excel
=CONTAR.BLANCO(H2:H21)
```

**Resultado:** 1 registro incompleto.

Se identificó que el registro del paciente P016 no contiene una medición de saturación de oxígeno.

La detección de este dato faltante evidencia la importancia de verificar la integridad de la información clínica antes de utilizarla para realizar análisis o apoyar decisiones.

## 4. Análisis y hallazgos clínicos

### 4.1. Estado de resolución de las consultas

De los 20 registros analizados, 9 corresponden a consultas finalizadas, equivalentes al 45 % del total.

Por otra parte, 11 registros (55 %) corresponden a pacientes que continúan en atención o presentan un estado pendiente.

Esta distribución permite identificar oportunidades para revisar el flujo de atención y realizar seguimiento a los casos que todavía no han sido cerrados.

Es importante aclarar que estos porcentajes describen el estado de los registros en el conjunto de datos y no constituyen, por sí solos, una medida definitiva de la eficiencia del servicio.

### 4.2. Casos que requieren atención prioritaria

**Paciente P009**

- **Sexo:** Femenino.
- **Edad:** 72 años.
- **Hallazgo registrado:** Dificultad respiratoria.
- **Frecuencia cardíaca:** 110 latidos por minuto (lpm).
- **Saturación de oxígeno:** 91 %.

La combinación de dificultad respiratoria, frecuencia cardíaca elevada y saturación de oxígeno reducida representa una señal de alerta clínica importante. En un contexto asistencial real, este cuadro requeriría valoración inmediata por el personal de salud y priorización según el protocolo de triaje correspondiente.

**Paciente P012**

- **Sexo:** Masculino.
- **Edad:** 61 años.
- **Hallazgo registrado:** Dolor torácico en estudio.
- **Saturación de oxígeno:** 94 %.

El dolor torácico requiere una evaluación clínica oportuna para determinar su causa y descartar condiciones potencialmente graves. La saturación registrada debe interpretarse junto con los síntomas, los antecedentes y los demás parámetros clínicos.

**Importante:** Estos hallazgos corresponden a un ejercicio académico con datos simulados. No representan diagnósticos médicos definitivos.

### 4.3. Integridad de la base de datos

Se detectó un dato faltante en el registro del paciente P016, correspondiente a la saturación de oxígeno.

La ausencia de esta medición limita la interpretación completa de las constantes vitales del registro. En un sistema de información hospitalario real, sería importante verificar si el dato no fue medido, no fue registrado o no estuvo disponible durante la atención.

Para mejorar la calidad de la información, se recomienda:

- Implementar mecanismos de validación de los campos clínicos.
- Identificar claramente los datos faltantes.
- Verificar la información antes de realizar cálculos estadísticos.
- Evitar asignar valores supuestos a mediciones que no fueron registradas.
- Establecer procedimientos de revisión para garantizar la consistencia de la base de datos.

## 5. Resumen de resultados

| Indicador | Resultado |
|---|---:|
| Total de registros | 20 pacientes |
| Edad promedio | 43,0 años |
| Temperatura promedio | 37,15 °C |
| Pacientes de sexo femenino | 10 (50 %) |
| Pacientes de sexo masculino | 10 (50 %) |
| Consultas finalizadas | 9 (45 %) |
| Pacientes en atención | 7 (35 %) |
| Pacientes pendientes | 4 (20 %) |
| Saturación de oxígeno mínima registrada | 91 % |
| Registros sin saturación de oxígeno | 1 (P016) |

6. Conclusiones

6.1. Análisis de datos

Excel permitió organizar los 20 registros y obtener indicadores para interpretar la información clínica.

6.2. Alertas clínicas

Los casos P009 y P012 presentaron datos que requieren especial atención y valoración médica.

6.3. Calidad de la información

El dato faltante de saturación de oxígeno del paciente P016 evidencia la importancia de registrar y verificar toda la información.

6.4. Gestión de la atención

La clasificación de los estados de atención facilita el seguimiento de los pacientes y la identificación de casos pendientes.
