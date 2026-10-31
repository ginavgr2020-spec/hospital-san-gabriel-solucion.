# Análisis de los registros clínicos simulados

**Estudiante:** Gina Valentina Gómez Rivadeneira  
**Proyecto:** Análisis de registros clínicos simulados  
**Herramienta utilizada:** Microsoft Excel  
**Tipo de datos:** Registros clínicos simulados con fines académicos  

## 1. Interpretación de los siete indicadores

La base contiene **20 registros de pacientes**. Los resultados siguientes describen únicamente los datos incluidos en el archivo y no representan conclusiones sobre una población real.

### Indicador 1. Total de pacientes

Se identificaron 20 registros, codificados desde P001 hasta P020. Este total constituye el conjunto utilizado para calcular los demás indicadores.

### Indicador 2. Edad promedio

La edad promedio es de **43 años**. Esto significa que la media de las edades registradas se encuentra en ese valor. La media ofrece una descripción general, pero no indica por sí sola cómo se distribuyen las edades ni permite caracterizar individualmente a los pacientes.

### Indicador 3. Temperatura promedio

La temperatura promedio es de **37,145 °C**. Es un resumen de las 20 mediciones registradas. Debe interpretarse como un indicador descriptivo del conjunto y no como una valoración clínica individual; para ello se necesitarían los antecedentes, síntomas y demás datos de cada paciente.

### Indicador 4. Distribución por sexo

Se registraron **10 mujeres (50 %) y 10 hombres (50 %)**. La distribución está equilibrada entre las dos categorías consignadas en la base. Este resultado describe exclusivamente el campo «Sexo» tal como fue diligenciado.

### Indicador 5. Estado de atención

De los 20 registros, **9 tienen la atención finalizada (45 %), 7 están en atención (35 %) y 4 están pendientes (20 %)**. La mayor proporción corresponde a atenciones finalizadas. La distribución permite conocer el estado administrativo o asistencial consignado, pero no informa por sí sola sobre la evolución clínica de los pacientes.

### Indicador 6. Saturación mínima de oxígeno

La saturación mínima registrada corresponde al paciente **P009**, con un valor de **0,91, equivalente a 91 %**. En ese mismo registro aparece dificultad respiratoria y una frecuencia cardíaca de 110 lpm. La combinación de estos datos representa una posible alerta que, en un contexto clínico real, requeriría valoración por personal de salud. El ejercicio no permite establecer un diagnóstico.

### Indicador 7. Datos faltantes de saturación

Se encontró **un registro sin dato de saturación de oxígeno**, correspondiente al paciente **P016**. La ausencia limita el análisis de ese indicador para dicho registro. No debe sustituirse el valor faltante por una estimación; si existiera una fuente original, se debería verificar allí.

## 2. Inconsistencias y situaciones que requieren revisión

En la revisión de la hoja se observaron los siguientes aspectos:

- **Dato faltante:** P016 no tiene un valor registrado en «saturación de oxígeno (%)». Debe conservarse como dato ausente hasta que pueda verificarse en una fuente válida.
- **Formato de saturación:** los valores están almacenados como fracciones decimales (por ejemplo, 0,91) aunque el encabezado los presenta como porcentaje. Para evitar confusiones, se debe documentar que 0,91 equivale a 91 %, o convertir toda la columna a una escala porcentual de manera uniforme. No se deben mezclar ambas escalas.
- **Mayúsculas y minúsculas:** el campo «diagnóstico simulado» contiene diferencias de escritura, por ejemplo, «cefalea» y «Cefalea» o «control preventivo» y «Control preventivo». Conviene unificar la presentación sin modificar el significado.
- **Espacios y encabezados:** algunos encabezados presentan espacios iniciales o caracteres de espacio no estándar. Esto puede dificultar filtros, fórmulas y análisis posteriores; se recomienda normalizarlos.
- **Contenido adicional en la hoja:** después de los 20 pacientes aparecen filas de resumen y datos para gráficos. No son registros individuales y deben excluirse del rango utilizado para calcular los indicadores, para evitar que se cuenten como pacientes.
- **Alertas para revisión clínica:** P009 presenta dificultad respiratoria, saturación de 91 % y frecuencia cardíaca de 110 lpm. P012 registra dolor de pecho. Son situaciones que, en un entorno real, ameritarían valoración oportuna. No constituyen diagnósticos definitivos.

Estas observaciones corresponden a calidad, formato e interpretación de los datos. Los resultados son descriptivos y dependen de la integridad de la información disponible.

## 3. Reflexión sobre la privacidad clínica

La privacidad clínica protege la información personal y de salud de cada paciente. Estos datos deben utilizarse únicamente para fines autorizados y su acceso debe limitarse a quienes los necesitan para cumplir sus funciones. También es importante evitar compartir archivos con información identificable, utilizar contraseñas y mantener los documentos en espacios seguros. En los trabajos académicos, el uso de registros ficticios permite practicar la organización y el análisis de información sin exponer datos de personas reales. Como futuros profesionales de la salud, debemos comprender que la confidencialidad no es un trámite, sino una responsabilidad ética. Incluso cuando los datos se presentan sin nombres, es necesario revisar qué información se comparte y con quién, para reducir riesgos de divulgación o uso inadecuado.

## 4. Conclusión

El análisis de los 20 registros permitió interpretar los siete indicadores solicitados, reconocer un dato faltante y detectar aspectos de formato que deben documentarse o normalizarse. También permitió identificar dos registros que, en un escenario real, requerirían revisión clínica. Los resultados deben entenderse como un ejercicio académico descriptivo basado en datos simulados.

**Declaración:** todos los registros son ficticios y se utilizan exclusivamente con fines académicos. Este análisis no sustituye la valoración de profesionales de la salud.
