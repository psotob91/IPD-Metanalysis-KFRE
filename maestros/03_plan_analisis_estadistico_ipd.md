# Plan de análisis estadístico para el IPD meta-analysis

## Estrategia analítica principal: Validación del modelo original

El análisis principal consistirá en la validación externa del modelo pronóstico original, cuyo propósito es evaluar su desempeño predictivo sin alterar la ecuación subyacente. La validación se diferencia estrictamente de la recalibración o actualización, ya que cuantificará la precisión de las predicciones utilizando los coeficientes, el intercepto y la estructura original del modelo, aplicados directamente sobre los datos no utilizados en su desarrollo 1, 2\.

## Descripción de participantes, case-mix y datos faltantes

Previo al modelamiento, se describirá de forma exhaustiva la cohorte analítica, detallando los participantes, las tasas de eventos observados y los tiempos de seguimiento estratificados por país y por cluster (centro u hospital). Se caracterizará la variabilidad de la casuística (*case-mix*) evaluando la distribución de los valores de los predictores en cada población, ya que los cambios en el case-mix constituyen una fuente primaria de heterogeneidad en el desempeño predictivo 3, 4\. Adicionalmente, se documentará la frecuencia y el patrón de valores faltantes (esporádicos y sistemáticos) para cada variable a nivel de cluster y país 5, 6\.

## Cálculo de predicciones

El riesgo absoluto individual se estimará aplicando con estricta fidelidad la arquitectura del modelo original. El cálculo ingresará los valores observados de los participantes en la ecuación, incorporando el intercepto o la función de riesgo basal original, los coeficientes (pesos) de los predictores, las transformaciones no lineales correspondientes (por ejemplo, uso de logaritmos o splines) y cualquier término de interacción especificado en la derivación inicial 7-9. En el caso de modelos de supervivencia, el cálculo se ajustará rigurosamente al horizonte de predicción temporal para el cual fue diseñado el modelo original, empleando la probabilidad de supervivencia basal en dicho punto temporal 10, 11\.

## Desempeño global, calibración y discriminación

La validación se sustentará en la evaluación del acuerdo entre las predicciones y los desenlaces observados, así como en la capacidad de separación de riesgos 12:

* **Calibración y desempeño global:** La calibración general se cuantificará mediante la relación entre el número de eventos Esperados y Observados (estadístico E/O o *calibration-in-the-large*), donde un valor ideal es 1 12, 13\. Adicionalmente, se calculará la pendiente de calibración (*calibration slope*), que evalúa si la propagación de los riesgos predichos es adecuada 12, 14\. Este desempeño se complementará visualmente mediante gráficos de calibración construidos con curvas suavizadas flexibles (loess o splines) que ilustren la concordancia a través de todos los deciles de riesgo predicho 15\.  
* **Discriminación:** Se medirá la capacidad del modelo para diferenciar a los individuos que presentan el desenlace de los que no. Para desenlaces binarios a corto plazo, se utilizará el área bajo la curva (AUC o estadístico C); para desenlaces de tiempo al evento, se calculará el índice de concordancia o estadístico D 16-18.  
* Todos los estadísticos se acompañarán de sus respectivos intervalos de confianza del 95% y se presentarán de forma global y desglosada por país y cluster 19, 20\.

## Consideración del clustering y síntesis del desempeño

Para acomodar la estructura jerárquica del consorcio de datos, la síntesis del desempeño predictivo no deberá ignorar el agrupamiento clínico 8\. Se utilizará un enfoque analítico (ya sea un meta-análisis de un paso *one-stage* estratificado o de dos pasos *two-stage* mediante meta-análisis de estimaciones por cluster) para resumir el desempeño global 21\. Dado que el nivel jerárquico superior cuenta con tan solo tres países, no se modelará la heterogeneidad entre países mediante enfoques convencionales de efectos aleatorios por su falta de robustez y asunciones de normalidad no verificables 22\. En su lugar, las diferencias a nivel de país se abordarán como efectos fijos o mediante la estimación estratificada del intercepto, limitando los términos de efectos aleatorios exclusivamente a las variaciones entre los clusters (centros/hospitales) dentro de cada país 23, 24\.

## Heterogeneidad y transportabilidad

La variabilidad del desempeño predictivo a través de los centros clínicos se evaluará sistemáticamente para determinar la generalizabilidad y transportabilidad del modelo. La heterogeneidad entre los clusters se ilustrará gráficamente mediante diagramas de bosque (*forest plots*) y diagramas de embudo (*funnel plots*), evaluando la precisión del modelo en relación al tamaño del cluster o la cantidad de eventos 20, 25\. Para evaluar empíricamente la transportabilidad geográfica, se ejecutará una validación cruzada interna-externa cíclica (*internal-external cross-validation*, IECV) 26, 27\. De manera iterativa, se excluirán todos los datos de un cluster (leave-one-cluster-out) o de un país entero (leave-one-country-out), aplicando el modelo sobre la cohorte omitida para documentar su consistencia en poblaciones totalmente independientes 28, 29\.

## Manejo de valores faltantes

El plan analítico asumirá que los datos faltan al azar (MAR) y se apoyará en técnicas de Imputación Múltiple para recuperar observaciones omitidas, preservando el poder estadístico 30\. Para los predictores parcial y sistemáticamente faltantes (ausentes por completo en algunos hospitales o países), se implementará un enfoque de Imputación Múltiple Multinivel (MLMI) que respete la agrupación y heterogeneidad entre los estudios durante el modelo de imputación 31, 32\. Como método complementario frente a predictores sistemáticamente faltantes, se podrá recurrir al modelado predictivo de ensamblaje (ensemble modeling), derivando predicciones específicas en cada estudio y combinándolas en un pronóstico final ponderado 33, 34\. Una vez realizadas las imputaciones, las métricas predictivas y los estadísticos de desempeño se consolidarán integrando los resultados a través de los conjuntos de datos mediante las reglas de combinación de Rubin 35, 36\.

## Análisis de sensibilidad

Se ejecutarán múltiples análisis de sensibilidad para confirmar la robustez de los hallazgos ante diferentes escenarios metodológicos:

1. **Casos completos:** Se realizará un análisis de casos completos (CCA) excluyendo individuos y clusters con datos faltantes, para evaluar posibles diferencias con los resultados de la imputación 37, 38\.  
2. **Armonización:** Se probarán escenarios secundarios alterando los puntos de corte o definiciones armonizadas para predictores clave o periodos de seguimiento.  
3. **Calidad y tamaño de los clusters:** Se recalculará el desempeño global excluyendo iterativamente clusters muy pequeños (ej. menos de 100 eventos) o aquellos con la mayor proporción de datos faltantes documentados 39, 40\.  
4. **Riesgos competitivos:** Si el tiempo al evento lo demanda, se incluirán estimaciones que contabilicen eventos competitivos específicos de la cohorte de validación que impidan la observación del desenlace principal 41\.

## Recalibración y actualización secundaria

Si el análisis principal de validación muestra un desempeño deficiente de la herramienta predictiva, específicamente reflejado en una pobre calibración sistemática, se procederá a implementar estrategias estructuradas de actualización del modelo (*model updating*) 42, 43\. Como primer nivel de actualización, se realizará una recalibración del intercepto (o actualización del riesgo basal) para ajustar las probabilidades base a las incidencias reales específicas de las poblaciones de los tres países de Latinoamérica 43, 44\. Si persiste una sobreestimación o subestimación desproporcionada de los riesgos a lo largo del espectro de predicción, se actualizará secundariamente la pendiente global de calibración (*calibration slope*). La reestimación individual de los coeficientes del modelo original o la adición de predictores locales suplementarios solo se considerará justificada si, tras la recalibración basal, la capacidad de discriminación se mantiene insuficiente y clínicamente inoperante 45, 46\.

## Software, reproducibilidad y control del código

En adherencia a los estándares de ciencia abierta, todo el flujo de trabajo —desde la preparación y limpieza de la base de datos hasta el análisis de meta-análisis y desempeño— se desarrollará utilizando el lenguaje estadístico estructurado R 47, 48\. Se utilizarán paquetes estandarizados y avalados como lme4 o sus equivalentes para modelamiento mixto 48, y paqueterías dedicadas como mice o micemd para los algoritmos de imputación múltiple 37, 49\. El conjunto completo de scripts, reglas sintácticas para la armonización y el código de cálculo predictivo estarán sujetos a control de versiones y serán reportados y publicados en formato *open-source* o repositorios públicos para asegurar la reproducibilidad técnica completa, cumpliendo con los estándares estipulados por la declaración TRIPOD-Cluster 50, 51\.  
