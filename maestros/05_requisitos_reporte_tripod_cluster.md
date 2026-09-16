# Requisitos de reporte metodológico según TRIPOD-Cluster y guías asociadas

## Título y resumen

**Qué debe prespecificarse:** El protocolo debe identificar claramente que el estudio es una evaluación o validación de un modelo de predicción multivariable utilizando datos agrupados o estructurados en clústeres (IPD meta-analysis). Debe especificar la población objetivo y el desenlace.**Diferenciación con el reporte final:** El protocolo establece el plan de diseño; el reporte final deberá incluir en el resumen las estimaciones clave del desempeño predictivo (calibración y discriminación) y sintetizar la heterogeneidad encontrada a través de los clústeres y países 1\.**Redacción modelo:**  
Validación externa y actualización del modelo pronóstico Nombre mediante un meta-análisis de datos individuales de participantes (IPD-MA) procedentes de múltiples clústeres en tres países latinoamericanos: protocolo de estudio. El objetivo es evaluar el desempeño predictivo frente al Desenlace.

## Antecedentes y objetivos

**Qué debe prespecificarse:** La justificación clínica y metodológica de validar el modelo utilizando IPD de tres países, destacando las ventajas de este diseño (mayor variabilidad del case-mix, aumento del tamaño muestral) para probar la transportabilidad del modelo. Debe definir si los objetivos se limitan a la validación externa o si contemplan la actualización 1-3.**Diferenciación con el reporte final:** El reporte final discutirá cómo los hallazgos empíricos responden a estos objetivos iniciales y justificará retrospectivamente la necesidad de actualización si el modelo falló.**Redacción modelo:**  
Este IPD-MA tiene como objetivo primario validar externamente el modelo original, evaluando su calibración y discriminación. El objetivo secundario es explorar la heterogeneidad del desempeño entre los distintos hospitales y países y, de ser necesario, recalibrar el modelo para optimizar su utilidad clínica en estos nuevos contextos geográficos.

## Diseño, países y fuentes de datos

**Qué debe prespecificarse:** El diseño del estudio observacional y el origen planificado de los datos. Se debe detallar el proceso de identificación, solicitud y consolidación de las bases de datos de los tres países, reconociendo la naturaleza agrupada (multinivel) de la información 4\.**Diferenciación con el reporte final:** El reporte publicará el diagrama de flujo final detallando exactamente cuántos clústeres y pacientes se identificaron, cuáles aportaron datos y cuántos se analizaron realmente tras la depuración 5\.**Redacción modelo:**  
El estudio emplea un diseño de validación externa basado en un IPD-MA observacional. Las fuentes de datos provienen de registros electrónicos de salud de tres países, estructuradas jerárquicamente en pacientes anidados dentro de hospitales/centros, consolidando una base de datos multinacional.

## Participantes, tiempo cero y elegibilidad

**Qué debe prespecificarse:** Los criterios de inclusión y exclusión a nivel de participantes y de clústeres. El "tiempo cero" o momento de inicio del seguimiento debe quedar unificado y definido a priori para evitar sesgos temporales 3, 4\.**Diferenciación con el reporte final:** El manuscrito final deberá presentar una tabla comparativa de las características basales de los pacientes en la cohorte de derivación original frente a las de las nuevas cohortes agrupadas por país y clúster 5\.**Redacción modelo:**  
Los criterios de elegibilidad se han armonizado para coincidir con la cohorte de desarrollo original. El tiempo cero se establece uniformemente como el momento de la admisión clínica. Se excluirán los clústeres que carezcan de variables mínimas o presenten deficiencias sistemáticas irresolubles de seguimiento.

## Desenlace, horizonte y predictores

**Qué debe prespecificarse:** La definición clínica exacta del evento a predecir, el horizonte de predicción (ventana temporal) y la lista de todos los predictores evaluados, especificando sus métodos y momentos de medición estandarizados 4\.**Diferenciación con el reporte final:** El artículo documentará retrospectivamente cualquier diferencia o variación real en la medición de predictores o desenlaces encontrada en la recolección de los datos de los clústeres respecto a los datos de desarrollo 4\.**Redacción modelo:**  
El desenlace primario, definido unificadamente como Evento clínico, se evaluará a los X años. Todos los predictores del modelo original serán extraídos, documentando exhaustivamente cualquier variación en los ensayos de laboratorio o definiciones institucionales locales antes de su armonización.

## Especificación del modelo

**Qué debe prespecificarse:** La ecuación predictiva completa original, incluyendo la función de riesgo basal (intercepto), los coeficientes asignados a cada predictor, y cualquier transformación o término de interacción especificado en su desarrollo 4\.**Diferenciación con el reporte final:** Tras el análisis, el reporte debe presentar de manera transparente el modelo final actualizado (si hubo recalibración), proveyendo los nuevos interceptos y explicando cómo calcular riesgos absolutos en nuevos individuos 6\.**Redacción modelo:**  
Se evaluará la ecuación del modelo de regresión Logística/Cox original. El riesgo individual se calculará insertando los valores de los pacientes en el predictor lineal compuesto por los coeficientes fijos originales y el intercepto reportado de X.

## Tamaño de muestra y precisión

**Qué debe prespecificarse:** La justificación metodológica de la idoneidad estadística de las bases combinadas, apuntando al cumplimiento de un mínimo efectivo de eventos por país y clúster (ej. mínimo de 100 a 200 eventos por estrato para una calibración robusta) 7\.**Diferenciación con el reporte final:** Se reportará la cantidad real de participantes, eventos, tiempos de seguimiento y censura en el total y desglosado obligatoriamente por cada clúster evaluado 5\.**Redacción modelo:**  
Se considera que la agregación multinacional aportará el poder estadístico necesario. Cada estrato analítico o país evaluado deberá superar el umbral de 100 eventos y 100 no-eventos para garantizar la precisión en las estimaciones de la pendiente de calibración.

## Armonización, calidad y faltantes

**Qué debe prespecificarse:** La estrategia formal para mapear variables clínicas dispares y el tratamiento estadístico para imputar datos esporádica y sistemáticamente faltantes respetando el clustering (ej. MLMI) 4, 8, 9\.**Diferenciación con el reporte final:** Se reportará transparentemente el número de observaciones faltantes por variable y clúster, y se describirán las características de convergencia del modelo de imputación y las variaciones con análisis de casos completos 5\.**Redacción modelo:**  
Los datos crudos se consolidarán en un diccionario unificado previo control de calidad. Los valores faltantes se manejarán mediante Imputación Múltiple Multinivel (MLMI) para abordar las ausencias sistemáticas, asumiendo un mecanismo de perdidos al azar (MAR) y preservando en la imputación la heterogeneidad basal y las interacciones del modelo analítico.

## Análisis estadístico

**Qué debe prespecificarse:** Las métricas de desempeño clínico que guiarán la evaluación. Esto incluye el índice C (discriminación) y estadísticas como el ratio E/O, la pendiente de calibración y curvas de suavizado (calibración), aplicando enfoques de meta-análisis para datos anidados 4, 10-12.**Diferenciación con el reporte final:** Las estimaciones se reportarán provistas de sus intervalos de confianza o predicción al 95%, proyectando la incertidumbre tanto globalmente como por cada unidad hospitalaria 6\.**Redacción modelo:**  
El desempeño del modelo no será simplemente agrupado (stacking naive). La validación se ejecutará midiendo la discriminación (Estadística C) y calibración (Ratio E/O y curvas flexibles loess). Las estimaciones globales de desempeño se consolidarán respetando los clústeres como efecto aleatorio o mediante un análisis meta-analítico de estimaciones por país.

## Clustering, heterogeneidad y transportabilidad

**Qué debe prespecificarse:** El enfoque para explorar y cuantificar cómo el desempeño varía entre los clústeres. Se predefinirá el uso de técnicas como la validación cruzada interna-externa cíclica y diagramas de bosque/embudo para estimar la transportabilidad 5, 10, 13\.**Diferenciación con el reporte final:** Se reportarán rigurosamente los intervalos de predicción del 95% para mostrar el grado real de generalizabilidad y se discutirá si las variaciones impiden una recomendación de uso global 6, 14, 15\.**Redacción modelo:**  
La variabilidad en el desempeño predictivo se evaluará explícitamente entre países y hospitales. Se utilizará una validación cruzada interna-externa cíclica, excluyendo iterativamente un clúster o país para someterlo a prueba. Esto cuantificará la verdadera transportabilidad geográfica ante las distintas prevalencias y distribuciones del case-mix.

## Recalibración o actualización

**Qué debe prespecificarse:** Las reglas exactas bajo las cuales se dictaminará si el modelo necesita ser adaptado. Debe distinguirse la validación estricta (usar ecuación intacta) de la actualización escalonada (ej. ajustar riesgo basal antes de tocar coeficientes) 5, 16\.**Diferenciación con el reporte final:** El manuscrito reportará obligatoriamente los resultados paralelos: el desempeño deficiente previo a la intervención y el desempeño mejorado posterior a las estrategias de recalibración, suministrando los nuevos valores paramétricos 6\.**Redacción modelo:**  
Si la validación externa demuestra infraestimación o sobreestimación sistemática de los riesgos, se procederá con una actualización del modelo local. Esta fase iniciará con la recalibración del riesgo basal específico por país (intercepto) para corregir discordancias en la prevalencia, restringiendo la reestimación total de coeficientes fijos a escenarios de fallo discriminativo severo.

## Riesgo de sesgo y aplicabilidad

**Qué debe prespecificarse:** Las herramientas validadas (como PROBAST) que se emplearán prospectivamente para auditar los defectos metodológicos y problemas de aplicabilidad de la cohorte original y de las bases de validación aportadas 4, 17\.**Diferenciación con el reporte final:** Se entregará un reporte tabular detallando las puntuaciones de riesgo de sesgo en cada clúster evaluado y se discutirán las implicaciones de esto en los análisis de sensibilidad preplanificados 18\.**Redacción modelo:**  
El riesgo de sesgo inherente a los registros electrónicos y bases de datos agrupadas se evaluará sistemáticamente para cada clúster mediante la herramienta PROBAST. Se ejecutarán análisis de sensibilidad subsiguientes excluyendo aquellas unidades con riesgo de sesgo alto que comprometan la inferencia estadística del desempeño.

## Ética, gobernanza, reproducibilidad y difusión

**Qué debe prespecificarse:** Las declaraciones de manejo seguro de datos internacionales, requerimientos regulatorios, software estadístico preseleccionado y plan de diseminación con apertura de código 19\.**Diferenciación con el reporte final:** El artículo proporcionará las rutas directas a los repositorios con los scripts de análisis (ej. R), declaraciones de conflictos de interés, el rol exacto de los financiadores y los apéndices suplementarios con el diccionario armonizado 19\.**Redacción modelo:**  
El consorcio de IPD contará con la aprobación de los respectivos Comités de Ética. Para garantizar plena transparencia, todos los procesos se documentarán adheridos a la guía TRIPOD-Cluster. El software estadístico R respaldará el modelado, y los algoritmos analíticos serán subidos a un repositorio público con control de versiones para facilitar el escrutinio abierto y la reproducibilidad científica por parte de la comunidad investigadora y los formuladores de políticas de salud latinoamericanos.  
