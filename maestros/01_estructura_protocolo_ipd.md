# Estructura y contenido recomendado para un protocolo de IPD meta-analysis de un modelo pronóstico

## Título y resumen

**Propósito:** El título debe identificar claramente el diseño metodológico (meta-análisis de datos individuales de participantes), el modelo pronóstico y la naturaleza multinivel de los datos. El resumen debe sintetizar el objetivo de la validación, las fuentes de datos y las técnicas analíticas principales.**Redacción modelo sugerida:**  
Validación externa y actualización del modelo pronóstico multivariable para la predicción de Desenlace utilizando datos agrupados de tres países latinoamericanos: protocolo de un meta-análisis de datos individuales de participantes (IPD-MA).**Resumen:** Este protocolo describe el marco metodológico para validar y, de ser necesario, actualizar un modelo clínico predictivo utilizando una cohorte multinacional. Se evaluará el desempeño predictivo del modelo original y se abordará la heterogeneidad entre los distintos centros y países mediante técnicas de imputación múltiple multinivel y modelado de efectos aleatorios.

## Antecedentes y justificación

**Propósito:** Explicar el contexto clínico, detallar por qué el modelo requiere una validación externa formal y justificar el enfoque de IPD-MA para evaluar la generalizabilidad del modelo en las nuevas poblaciones.**Redacción modelo sugerida:**  
La mayoría de los modelos predictivos publicados carecen de una validación externa robusta, lo cual limita su adopción en la práctica clínica 1, 2\. La validación en datos independientes es fundamental, ya que el rendimiento predictivo tiende a sobreestimarse en los datos de desarrollo 1\. La combinación de datos individuales de participantes (IPD) provenientes de múltiples estudios o registros electrónicos de salud proporciona una oportunidad única para validar modelos de manera externa 3, 4\. Este enfoque de IPD-MA permite evaluar directamente la generalizabilidad del modelo pronóstico a través de diversas poblaciones y subgrupos, y ofrece el poder estadístico necesario para detectar y abordar la heterogeneidad en el desempeño predictivo entre los distintos centros médicos de los países de América Latina participantes 5, 6\.

## Descripción del modelo pronóstico evaluado

**Propósito:** Especificar detalladamente la arquitectura del modelo original que será sometido a validación, incluyendo su formato estadístico y las variables que lo componen.**Redacción modelo sugerida:**  
El modelo pronóstico a evaluar se desarrolló originalmente mediante una regresión multivariable. La arquitectura del modelo proporciona una ecuación que estima el riesgo absoluto de un individuo basándose en una combinación de múltiples características clínicas 7\. La ecuación incluye un término de riesgo basal (intercepto o riesgo base) combinado con los efectos (coeficientes) de los siguientes predictores: Lista de predictores. El riesgo individual absoluto se calcula ingresando los valores de los predictores del paciente en la ecuación original y transformando el resultado a una escala de probabilidad 8\.

## Objetivos primario y secundarios

**Propósito:** Diferenciar claramente los fines evaluativos (validación) de los fines adaptativos (actualización) u otros análisis secundarios del IPD-MA.**Redacción modelo sugerida:**  
El objetivo primario es realizar una validación externa del modelo pronóstico, examinando el acuerdo entre los riesgos predichos y los observados (calibración) y su capacidad para separar a los individuos con y sin el desenlace (discriminación) en los datos no utilizados en su desarrollo original 1, 9\. Los objetivos secundarios incluyen: 1\) cuantificar la heterogeneidad del desempeño del modelo entre los distintos países, hospitales y centros participantes 6; y 2\) actualizar o recalibrar el modelo para adaptarlo al riesgo basal específico de estas poblaciones, en caso de que la validación demuestre un rendimiento subóptimo o sesgos sistemáticos en las predicciones originales 10, 11\.

## Diseño del estudio

**Propósito:** Describir la estrategia epidemiológica general y adherencia a las guías de reporte estandarizadas para datos agrupados.**Redacción modelo sugerida:**  
El presente estudio consiste en un meta-análisis de datos individuales de participantes (IPD-MA) de carácter observacional retrospectivo. El diseño, análisis y posterior reporte de los resultados se estructuran siguiendo la directriz TRIPOD-Cluster (Transparent Reporting of a multivariable prediction model for Individual Prognosis or Diagnosis using clustered data) 12, 13, la cual provee estándares metodológicos específicos para estudios de modelos de predicción que utilizan bases de datos jerárquicas o anidadas.

## Fuentes de datos y países participantes

**Propósito:** Identificar la procedencia de los registros y destacar cómo la estructura del consorcio de datos enriquece la evaluación del modelo.**Redacción modelo sugerida:**  
Se consolidarán datos retrospectivos provenientes de bases de datos de registros médicos electrónicos e historiales clínicos de tres países de Latinoamérica. La integración de estos grandes conjuntos de datos (big data) provenientes de centros independientes representa una validación cruzada geográfica robusta y minimiza los riesgos de validaciones pequeñas y aisladas 4, 14\.

## Población objetivo

**Propósito:** Definir el universo de pacientes al que se pretende aplicar el modelo pronóstico en la práctica clínica diaria.**Redacción modelo sugerida:**  
La población objetivo está constituida por Descripción clínica de los pacientes en riesgo, para quienes las predicciones de riesgo guiarán las decisiones terapéuticas y de seguimiento preventivo 15\.

## Criterios de elegibilidad

**Propósito:** Establecer los criterios de inclusión y exclusión a nivel de participantes dentro de las bases de datos obtenidas.**Redacción modelo sugerida:**  
Se incluirán todos los individuos consecutivos registrados en los centros participantes que cumplan con los criterios diagnósticos iniciales de la cohorte original. Se excluirán aquellos pacientes en los que la información sobre el desenlace primario o el tiempo de seguimiento sea completamente inexistente, tras agotar los procesos de verificación de calidad de los datos 16, 17\.

## Momento de inicio o tiempo cero

**Propósito:** Estandarizar metodológicamente el inicio del horizonte predictivo para todos los participantes a través de los múltiples centros.**Redacción modelo sugerida:**  
El tiempo cero (baseline) se establece unificadamente como el momento de la confirmación del diagnóstico o la admisión clínica índice. Esta estandarización es esencial previo a la combinación de las fuentes de datos (stacking) para evitar que diferencias en el inicio del seguimiento afecten la interpretabilidad clínica del riesgo pronosticado 16, 18\.

## Desenlace y horizonte de predicción

**Propósito:** Detallar el evento clínico a predecir y el período de tiempo sobre el cual el modelo estima la probabilidad del riesgo.**Redacción modelo sugerida:**  
El desenlace a predecir es Evento clínico en un horizonte temporal de X años. Las definiciones del desenlace se armonizarán y unificarán a través de todos los países participantes para garantizar la consistencia, abordando así la heterogeneidad intrínseca que surge al utilizar grandes bases de datos de registros médicos rutinarios 19\.

## Predictores

**Propósito:** Listar las variables requeridas por el modelo y cómo se gestionarán las variaciones en las mediciones clínicas rutinarias.**Redacción modelo sugerida:**  
Se extraerán todos los predictores multivariables especificados por el modelo original. Se documentarán explícitamente las variaciones observadas en los diferentes entornos clínicos relativas a la definición de los predictores, el equipo de medición o los puntos de corte, dado que la heterogeneidad en los métodos de recolección puede impactar en la magnitud de los efectos de los predictores y, por ende, en el desempeño del modelo 16, 20\.

## Estructura jerárquica o agrupada de los datos

**Propósito:** Reconocer formalmente que los pacientes se agrupan en centros/países y plantear la necesidad estadística de tratar estos clústeres.**Redacción modelo sugerida:**  
Los datos subyacentes presentan una agrupación inherente, conformando una estructura jerárquica en la que los participantes están anidados dentro de centros u hospitales, los cuales se agrupan en regiones y países 21, 22\. Dado que las observaciones dentro del mismo clúster clínico tienden a ser más similares entre sí que las observaciones de diferentes clústeres, asumir erróneamente que todos los datos provienen de una única población homogénea (ignorar la agrupación o "stacking" ingenuo) genera conclusiones engañosas y proyecciones de generalizabilidad defectuosas 23, 24, 22\. El protocolo exige que todo análisis tome en cuenta explícitamente este nivel de agregación 25\.

## Adquisición, transferencia y gobernanza de los datos individuales

**Propósito:** Definir el marco regulatorio y logístico de la gestión de la información de los tres países.**Redacción modelo sugerida:**  
Tras la aprobación por parte de los comités de ética locales, los datos se solicitarán y transferirán de forma segura desde cada uno de los centros a un repositorio de coordinación central. Se implementarán acuerdos de transferencia y uso de datos que regulen la propiedad y el acceso a esta información unificada, promoviendo la colaboración para la investigación de la validación externa del modelo sin vulnerar los sistemas normativos locales 21\.

## Armonización de variables

**Propósito:** Establecer el proceso para unificar los datos provenientes de distintos sistemas y lenguajes clínicos.**Redacción modelo sugerida:**  
Los datos provenientes de distintas fuentes estarán sujetos a un riguroso proceso de armonización. Se desarrollará un diccionario de datos común y las variables crudas de los registros electrónicos de salud se mapearán y recodificarán a escalas uniformes. Esta estandarización metodológica pre-análisis mitiga el sesgo derivado del uso de sistemas de recolección dispares entre países 18, 19\.

## Verificación de calidad e integridad de los datos

**Propósito:** Controlar los posibles errores inherentes al uso de "big data" y registros electrónicos rutinarios.**Redacción modelo sugerida:**  
Se realizarán controles exhaustivos de la calidad de los datos para identificar ingresos atípicos, inconsistencias clínicas en las fechas de los eventos y falta de estandarización en las codificaciones diagnósticas, problemas frecuentes en registros médicos electrónicos no diseñados originalmente para investigación 26, 19\. Solo los datos validados tras estas comprobaciones se incluirán en las fases de imputación y análisis.

## Tamaño de muestra y precisión

**Propósito:** Justificar la suficiencia de la base de datos para la evaluación robusta del modelo, basado en el número de eventos observados.**Redacción modelo sugerida:**  
La solidez de los análisis de validación externa exige que la muestra analítica cuente con un mínimo riguroso de 100 eventos y 100 no-eventos por país o clúster de interés 27, 28\. Para análisis que evalúan detalladamente la calibración mediante estimaciones estratificadas, este requisito asciende preferiblemente a 200 eventos 28\. El IPD-MA garantiza la consecución y superación de este tamaño efectivo de la muestra al aglutinar registros de múltiples fuentes 27\.

## Valores faltantes

**Propósito:** Detallar el enfoque estadístico adoptado para manejar tanto las ausencias aleatorias (a nivel individual) como sistemáticas (a nivel de estudio/centro) de las variables.**Redacción modelo sugerida:**  
Para tratar los datos faltantes bajo la suposición de que los datos faltan al azar (MAR), se aplicarán técnicas avanzadas de Imputación Múltiple 29, 30\. Dado que es altamente probable encontrar predictores omitidos sistemáticamente en algunos hospitales o países enteros (systematically missing predictors), se descarta el uso del Análisis de Casos Completos (CCA) por su pérdida de poder estadístico y riesgo de sesgo 31, 32, así como métodos de imputación ingenuos que ignoren la heterogeneidad entre estudios 32\. En su lugar, se implementará la Imputación Múltiple Multinivel (MLMI) que contabiliza correctamente la variabilidad y estructura jerárquica 33, 34, o subsidiariamente, un enfoque predictivo de ensamblaje (ensemble modeling) que evalúe modelos ajustados localmente ignorando las variables omitidas sistemáticamente y luego sintetice sus predicciones en un pronóstico final ponderado 35, 36, 37\. Se generarán un mínimo de 20 a 50 conjuntos de datos imputados 38\.

## Análisis estadístico

**Propósito:** Presentar el marco de modelado multivariable que rige el IPD-MA, ajustando por clústeres.**Redacción modelo sugerida:**  
Las evaluaciones del modelo pronóstico original y sus posibles recalibraciones se realizarán ajustando modelos mixtos lineales generalizados o modelos de efectos aleatorios para incorporar y explicar la agrupación de los pacientes dentro de los centros u hospitales 33, 39\. El análisis estadístico contemplará explícitamente términos de efectos aleatorios para el intercepto (o riesgo basal) del modelo a fin de dar cabida a la varianza inherente en la incidencia del desenlace entre los distintos países y centros 40, 41\.

## Evaluación de calibración, discriminación y desempeño global

**Propósito:** Precisar qué métricas determinarán el desempeño inicial (validación externa).**Redacción modelo sugerida:**  
La validez del modelo se determinará mediante la medición de dos componentes fundamentales: discriminación y calibración 1\. La discriminación se evaluará utilizando el índice de concordancia (estadística C) que mide la capacidad del modelo para separar adecuadamente a los sujetos con y sin el desenlace clínico 42, 9\. La calibración se analizará comparando los riesgos pronosticados por el modelo frente a las probabilidades empíricas observadas. Las métricas incluirán la relación de eventos esperados sobre los observados (estadística E/O) y la pendiente de la calibración 43, 9\. Estos resultados se complementarán visualmente utilizando gráficos de calibración flexibles generados mediante curvas de suavizado (loess), proyectados de manera general y estratificada por deciles de riesgo predicho 43, 9\.

## Evaluación de heterogeneidad entre países y clusters

**Propósito:** Explicar cómo la validación irá más allá de un promedio global, examinando sistemáticamente la variabilidad en los resultados predictivos geográficamente.**Redacción modelo sugerida:**  
Más allá de reportar un rendimiento predictivo promedio a través de todos los datos combinados, se realizará un meta-análisis de efectos aleatorios para explorar y cuantificar de manera rigurosa la heterogeneidad en el desempeño del modelo entre los países y clústeres hospitalarios 44, 45\. Los resultados a nivel de clúster se visualizarán utilizando diagramas de bosque (forest plots) y diagramas de embudo (funnel plots) para métricas clave de validación como la estadística C y el índice E/O 46, 47, 48\. Además de la estadística I², la extensión real de la generalizabilidad entre las diferentes poblaciones en riesgo se sintetizará mediante la derivación de intervalos de predicción del 95%, revelando los límites dentro de los cuales es factible que caiga el desempeño del modelo en nuevos entornos de aplicación médica 49, 50\.

## Análisis de sensibilidad

**Propósito:** Declarar pruebas estadísticas complementarias para corroborar la resiliencia y consistencia de la evaluación.**Redacción modelo sugerida:**  
Se planificarán análisis de sensibilidad que examinarán si el desempeño discriminativo o la calibración del modelo cambian sustancialmente tras la modificación de supuestos metodológicos clave, como variaciones secundarias en los puntos de corte o definiciones de los predictores, o después de excluir deliberadamente aquellos centros clínicos con el mayor grado de datos faltantes documentados 51\. Adicionalmente, se podrá considerar un enfoque de validación cruzada interna-externa cíclica (leave-one-study-out) 52, 53 para poner a prueba iterativamente la transportabilidad geográfica de las estimaciones en distintas combinaciones de los centros estudiados 54\.

## Recalibración o actualización, cuando corresponda

**Propósito:** Demarcar claramente el momento de transición entre la evaluación (verificación) y la actualización clínica del modelo para adaptarlo a nuevas poblaciones.**Redacción modelo sugerida:**  
Si la validación externa evidencia que las predicciones originales no son directamente fiables a lo largo de las nuevas cohortes latinoamericanas, se debe distinguir entre la simple validación y las estrategias de actualización (model updating). A diferencia de la validación —que solo documenta la precisión estadística del modelo—, la recalibración es una forma de actualización o sintonización en la cual el modelo se modifica de manera estructurada para reflejar las realidades de la nueva población de pacientes 10, 11\. Si se detectan grandes niveles de heterogeneidad con infra o sobre-estimaciones sistemáticas (calibración deficiente), se procederá inicialmente con una actualización del intercepto del modelo o tasa de riesgo basal adaptándolo de manera específica por país o clúster para corregir las discordancias en la prevalencia 55, 11, 30\. Las técnicas de alteración o introducción de nuevos efectos predictores se restringirán solo para aquellos casos donde la discriminación global sea insuficientemente clínica y fallida 56, 57\.

## Riesgo de sesgo y aplicabilidad

**Propósito:** Cuantificar el peso de las imperfecciones metodológicas de los datos agrupados obtenidos.**Redacción modelo sugerida:**  
Todos los conjuntos de datos incluidos provenientes de las tres naciones serán sometidos a una evaluación de aplicabilidad y riesgo de sesgo estructurada y validada mediante la herramienta PROBAST (Prediction model Risk Of Bias ASsessment Tool) 58, 51, 59\. Esto resguardará la validez al certificar si existen desviaciones sistemáticas importantes debido al flujo de pacientes o técnicas de clasificación de eventos.

## Ética, privacidad y confidencialidad

**Propósito:** Especificar salvaguardas sobre información sanitaria compartida a nivel internacional.**Redacción modelo sugerida:**  
Todos los protocolos de recolección e integración de historiales clínicos requerirán la aprobación independiente por parte de los Comités de Ética Institucionales y de Investigación de los centros y países aportantes. Todos los datos individuales de pacientes serán rigurosamente despojados de cualquier identificador personal directo previo a su consolidación en el IPD-MA para proteger plenamente el derecho internacional de privacidad y confidencialidad 21\.

## Reproducibilidad, software y manejo del código

**Propósito:** Asegurar la disponibilidad comunitaria y repetibilidad en la ciencia de datos clínicos.**Redacción modelo sugerida:**  
Los análisis estadísticos descriptivos, los procesos de imputación múltiple multinivel, así como los algoritmos predictivos y el meta-análisis se ejecutarán en R de manera completamente trazable. Todos los conjuntos de scripts, algoritmos y procedimientos analíticos se subirán a repositorios científicos públicos u open-source pertinentes para avalar la plena transparencia científica y permitir su total reproducibilidad 59\.

## Plan de publicación y difusión

**Propósito:** Explicitar el estándar usado para diseminar los hallazgos en la comunidad médica.**Redacción modelo sugerida:**  
Los resultados de la validación clínica externa y posible actualización del modelo pronóstico serán documentados y publicados ciñéndose de manera estricta a la guía de publicación internacional de consenso TRIPOD-Cluster 12, 13, la cual estipula directrices exhaustivas sobre cómo reportar estudios de modelado predictivo multivariable procedentes de grandes bases de datos agrupadas. Los resultados se diseminarán a través de publicaciones en revistas de alto impacto con el fin de informar a los gestores de políticas sanitarias latinoamericanos sobre el uso seguro o la necesidad imperativa de adaptación local de la herramienta pronóstica evaluada 60, 61\.  
