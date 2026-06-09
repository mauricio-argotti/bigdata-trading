<!-- Convertido automáticamente desde PDF. Revisar y corregir formato si es necesario. -->

# Capítulo 1: Big Data y Análisis Multivariante

**Big Data y Análisis Multivariante para la Predicción de la Dirección del Precio en Mercados Financieros** 

## Introducción

```{figure} 01_big_data_images/1._Big_Data.png
---
width: 90%
name: fig-intro-big-data
align: center
---
Introducción al Big Data y Análisis Multivariante.
```


La creciente digitalización de los mercados financieros ha generado un ecosistema caracterizado por volúmenes masivos de datos, latencias reducidas y una diversidad creciente de fuentes de información. Este fenómeno, ampliamente documentado en la literatura reciente, ha impulsado el desarrollo de modelos predictivos basados en Big Data y aprendizaje automático para anticipar el movimiento direccional del precio de activos financieros. Sin embargo, la proliferación de modelos cada vez más complejos —como redes neuronales profundas, LSTM o Transformers— ha introducido un nuevo desafío: la pérdida de interpretabilidad y la dificultad para justificar decisiones de inversión basadas en modelos opacos. 

En paralelo, diversos estudios han demostrado que la acción del precio (price action) continúa siendo una de las fuentes más robustas y estables de información predictiva, especialmente en horizontes de corto plazo y en mercados altamente líquidos. No obstante, la abundancia de variables derivadas del precio genera redundancia, multicolinealidad y ruido, lo que compromete la estabilidad de los coeficientes y la capacidad de generalización de los modelos. 

Este TeachBook propone un enfoque alternativo: modelos parsimoniosos, interpretables y estadísticamente robustos, construidos a partir de análisis multivariante y técnicas de selección de variables aplicadas a grandes volúmenes de datos. El objetivo es proporcionar un marco metodológico que permita a traders cuantitativos, gestores de activos y equipos de investigación construir modelos predictivos que no solo sean precisos, sino también explicables y defendibles ante comités de riesgo, reguladores y revisores académicos. 

## **PANORAMA DE LOS MODELOS PREDICTIVOS** 

```{figure} 01_big_data_images/2._Problema_Actual.png
---
width: 90%
name: fig-problema-actual
align: center
---
Panorama actual de los modelos predictivos.
```

El mundo de los mercados financieros ha experimentado un cambio significativo con la llegada de la era de los datos masivos y la tecnología de aprendizaje automático. La capacidad de procesar grandes cantidades de datos en tiempo real ha permitido a los modelos predictivos mejorar su precisión y eficacia en la predicción de precios y detección de patrones de mercado. Sin embargo, la complejidad de estos datos y la falta de interpretabilidad de estos modelos plantean nuevos desafíos para los analistas y los inversores. 

La complejidad y volatilidad de los mercados financieros han llevado a la búsqueda de soluciones más efectivas para la predicción de precios y la toma de decisiones informadas. En este contexto, se presentan dos enfoques clave que han demostrado su capacidad para mejorar la precisión y eficiencia en la predicción de mercados financieros. 

La investigación contemporánea en modelización financiera se encuentra en un punto de inflexión marcado por la convergencia entre Big Data, aprendizaje automático y la necesidad creciente de modelos explicables. El uso de arquitecturas avanzadas, desde pipelines de datos de alta frecuencia hasta redes profundas capaces de capturar patrones no lineales, ha ampliado significativamente la capacidad predictiva en mercados complejos. Sin embargo, esta sofisticación técnica ha venido acompañada de desafíos críticos: opacidad, fragilidad ante cambios de régimen, sobreajuste y dificultades para justificar decisiones en entornos regulados. 

En este contexto, la acción del precio emerge nuevamente como una fuente primaria de información robusta, mientras que la gobernanza y la interpretabilidad de modelos se consolidan como requisitos esenciales para garantizar la fiabilidad operativa. Los siguientes apartados sintetizan los avances recientes y las tensiones metodológicas que definen el estado actual del campo. 

## **1. Modelos predictivos basados en Big Data** 

La literatura reciente destaca el uso de arquitecturas Big Data para procesar flujos masivos de datos financieros en tiempo real, integrando técnicas de aprendizaje automático para la predicción de precios y detección de patrones de mercado. Estos enfoques permiten manejar datos de alta frecuencia, profundidad de libro y señales alternativas, pero suelen carecer de interpretabilidad. 

## **2. Aprendizaje automático y deep learning en mercados financieros** 

Modelos como Random Forest, SVM, LSTM y Transformers han mostrado capacidad para capturar relaciones no lineales y patrones complejos en series temporales financieras. Sin embargo, estudios recientes advierten que su desempeño puede deteriorarse significativamente en presencia de cambios de régimen, ruido microestructural y sobreajuste, especialmente cuando no se aplican protocolos rigurosos de validación. 

## **3. Acción del precio como fuente primaria de información** 

La acción del precio sigue siendo una de las fuentes más estables y predictivas en mercados líquidos. Investigaciones recientes muestran que muchos indicadores técnicos derivados del precio no aportan información adicional significativa y pueden introducir redundancia y multicolinealidad, afectando la estabilidad de los modelos. 

## **4. Interpretabilidad y gobernanza de modelos** 

La creciente preocupación por la opacidad de los modelos ha impulsado el interés en enfoques explicables (XAI) y modelos lineales o semilineales que permitan comprender la relación entre variables predictoras y señales de trading. La literatura enfatiza la necesidad de modelos que combinen precisión con interpretabilidad, especialmente en contextos regulados y de alto riesgo operativo. 

## **5. Precisión vs interpretabilidad** 

La literatura reciente muestra que la predicción financiera moderna se mueve entre dos polos. Por un lado, arquitecturas Big Data y modelos de aprendizaje profundo capaces de procesar volúmenes masivos de información y capturar patrones no lineales. Por otro lado, la necesidad creciente de interpretabilidad, estabilidad y gobernanza en entornos donde el riesgo operativo es crítico. 

Aunque los modelos avanzados como Random Forest, SVM, LSTM y Transformers han demostrado un rendimiento notable en condiciones controladas, su fragilidad ante cambios de régimen, ruido microestructural y sobreajuste revela que la precisión histórica no garantiza robustez futura. En 

contraste, la acción del precio emerge como una fuente de información más estable y menos susceptible a distorsiones, mientras que muchos indicadores derivados introducen redundancia y degradan la calidad del modelo. 

A este panorama se suma un hallazgo transversal la complejidad no siempre se traduce en mejor capacidad predictiva, y en mercados financieros, la explicabilidad es un requisito operativo, no un lujo metodológico. La literatura converge en que los modelos deben equilibrar precisión y transparencia, integrando prácticas de validación rigurosa, reducción de dimensionalidad y técnicas XAI (Inteligencia Artificial Explicable) que permitan justificar decisiones en contextos regulados. 

Por otra parte, los estudios sugieren que el futuro de la predicción financiera no depende únicamente de modelos más sofisticados, sino de modelos más gobernables, auditables y resilientes, capaces de mantener un desempeño bajo condiciones cambiantes y de ofrecer señales comprensibles para la toma de decisiones. De este modo, el avance científico en el ámbito de la predicción financiera no depende únicamente de modelos más potentes, sino de modelos más responsables. La literatura converge en que la combinación óptima integra datos robustos (acción del precio), modelos parsimoniosos o explicables, validación estricta, y una gobernanza sólida del ciclo de vida del modelo. Este equilibrio es el que permite transformar precisión técnica en valor operativo real. 

## **CAPÍTULO 1 — FUNDAMENTOS TEÓRICOS Y METODOLÓGICOS** 

## **1.1. Big Data en Mercados Financieros** 

El uso de Big Data en los mercados financieros ha evolucionado de forma acelerada en la última década, impulsado por la digitalización de las operaciones bursátiles, la proliferación de fuentes de datos no estructurados y el avance de la computación de alto rendimiento. Hoy, las instituciones financieras, desde bancos de inversión hasta hedge funds cuantitativos, dependen de infraestructuras capaces de procesar volúmenes masivos de información en tiempo real para obtener ventajas competitivas en predicción, gestión de riesgos y ejecución algorítmica. En este contexto, las clásicas tres V del Big Data adquieren características específicas en el ámbito financiero, donde los requisitos técnicos y analíticos son especialmente exigentes. 

## **1.1.1. Las tres V del Big Data financiero** 

```{figure} 01_big_data_images/3._Torbellino_Big-Data.png
---
width: 90%
name: fig-torbellino-big-data
align: center
---
El torbellino del Big Data en finanzas.
```

- **Volumen** : millones de observaciones intradía y datos alternativos. 

En los mercados financieros modernos, el volumen de datos crece de forma exponencial. No solo se generan millones de observaciones intradía por activo, precios, volúmenes, órdenes, cancelaciones, sino que además se incorporan nuevas fuentes de datos alternativos (alternative data), como: 

- Geolocalización de dispositivos móviles, 

- Imágenes satelitales, 

- Registros de transacciones electrónicas, 

- Datos climáticos, 

- Actividad en redes sociales, 

- Métricas de comportamiento digital. 

Según estimaciones recientes, un fondo cuantitativo de tamaño medio puede procesar entre 1 y 10 terabytes diarios de datos brutos. Este crecimiento obliga a utilizar arquitecturas distribuidas (Hadoop, Spark), almacenamiento en la nube y técnicas de compresión y filtrado inteligente. 

## **Volumen de Datos (** 𝑉) 

La cantidad total de datos (𝑉) generados en un intervalo de tiempo (intervalo de análisis definido por el analista: un segundo, una hora, una sesión de mercado, etc). De acuerdo con (Gandomi 2015) la fórmula que mejor explica este criterio es: 

## 𝑉= 𝑁. 𝑆 

## Donde: 

𝑁 = Número de registros generados durante un intervalo de tiempo 

𝑆 = Tamaño promedio en bytes de cada registro. 

## _**Ejemplo**_ **:** 

Si en 1 segundo se generan 50000 ticks y cada tick ocupa 120 bytes, entonces el volumen de datos generado en un segunde es de 6 millones de bytes. 

• **Velocidad** : latencias de milisegundos y decisiones automatizadas. 

La velocidad es crítica en los mercados financieros, especialmente en estrategias de _high-frequency_ 

- _trading_ (HFT) y _market making_ . La competencia se mide en milisegundos o incluso microsegundos. 

   - Los sistemas de negociación deben procesar flujos de datos de mercado (market data feeds) con latencias inferiores a 1 ms. 

   - Las decisiones algorítmicas, detección de patrones, ejecución de órdenes, gestión de riesgo, se automatizan para evitar retrasos humanos. 

   - La infraestructura se optimiza mediante co-localización, redes de baja latencia y hardware especializado (FPGAs, GPUs). 

La velocidad no solo afecta a la ejecución, sino también al análisis: modelos de nowcasting, predicción intradía y detección de anomalías requieren pipelines de datos en streaming (Kafka, Flink) capaces de actualizar estimaciones en tiempo real. 

## **Velocidad de generación del dato (** 𝑉𝑒 **):** 

La velocidad de generación del dato es una métrica que cuantifica la rapidez con la que un sistema financiero produce eventos observables, como transacciones, actualizaciones en el libro de órdenes o cambios en el bid/ask, dentro de un intervalo de tiempo específico. Esta métrica permite evaluar la intensidad del flujo de información que un modelo predictivo o una arquitectura de Big Data debe procesar en tiempo real. Matemáticamente según (Chen, 2014), se define como: 

**==> picture [36 x 24] intentionally omitted <==**

Donde: 

𝑁 = Número de eventos generados o cambios observables en los flujos de datos (transacciones, actualización de órdenes, etc.) 

∆𝑡 = Intervalo de tiempo. 

## _**Ejemplo:**_ 

Supongamos que, en un intervalo de 1 segundo, se registraron 12,000 actualizaciones del libro de órdenes, 1,500 transacciones ejecutadas y 3,000 cambios en el bid/ask. Al calcular la velocidad de generación del dato **(** 𝑉𝑒 **)** , esto indica que se produjeron un total de 16,500 eventos en ese período, es decir, una tasa de 16,500 eventos por segundo. 

• **Variedad** : precios, volúmenes, noticias, sentimiento, derivados. La variedad de datos financieros ha aumentado drásticamente. Ya no basta con series temporales tradicionales, los modelos modernos integran múltiples tipos de información heterogénea: 

- **Datos estructurados** : precios, volúmenes, curvas de tipos, volatilidades implícitas. 

- **Datos semiestructurados** : libros de órdenes (LOB), mensajes FIX, reportes regulatorios. 

- **Datos no estructurados** : noticias económicas, informes corporativos, publicaciones en redes sociales, transcripciones de conferencias de resultados (earnings calls), sentimiento textual mediante NLP. 

La investigación reciente muestra que los modelos que combinan datos tradicionales con datos alternativos, por ejemplo, sentimiento de Twitter o análisis semántico de noticias, pueden mejorar la capacidad predictiva entre 5 % y 20 %, dependiendo del activo y el horizonte temporal. 

Además, la variedad incluye datos derivados de modelos: volatilidad realizada, indicadores de liquidez, embeddings generados por redes neuronales, etc. Esta diversidad exige técnicas avanzadas de integración, limpieza y alineación temporal. 

Desde el punto de vista del análisis de la variedad de los datos previo a la construcción de modelos predictivos, existen numerosas métricas útiles para dimensionar la importancia y la utilidad de los datos en este proceso. Algunas de las más relevantes, según Gandomi (2015), son: la cardinalidad de tipos de datos, el índice de complejidad estructural, la entropía de Shannon para datos textuales, la dimensionalidad efectiva para datos numéricos y la diversidad de fuentes independientes. Aunque todas estas métricas aportan valor, la más crucial, aquella que realmente determina qué tipo de dato es útil para un modelo predictivo, es la dimensionalidad efectiva. 

## **Dimensionalidad efectiva (** _**D**_ ₑ **)** 

Según Jolliffe (2016), la dimensionalidad efectiva es el número real de dimensiones independientes en un conjunto de datos. Es una medida que refleja cuánta estructura informativa existe realmente, más allá de la redundancia, la correlación y el ruido presentes en los datos. En términos formales, la dimensionalidad efectiva corresponde al rango de la matriz de datos, es decir, al número de vectores columna linealmente independientes que aportan información única para la modelización. 

Sea X una matriz de datos de tamaño n x p, donde n = número de observaciones p = número de variables 

La dimensionalidad efectiva ( _D_ ₑ) se define como: 

𝐷𝑒 = 𝑟𝑎𝑛𝑘 (𝑋) 

Donde: 

rank (𝑋) = número de columnas linealmente independientes matemáticamente se calcula mediante: 

- Descomposición SVD 

- Descomposición QR 

- Eigenvalores de la matriz de covarianzas 

Equivalentemente: 

**==> picture [79 x 12] intentionally omitted <==**

Donde: 

𝜆𝑖 son los autovalores de la matriz de covarianzas 𝑋[𝑇] 𝑋 

## _**Ejemplo:**_ 

Supongamos que un analista construye un conjunto de datos con un total de 300 variables distribuidas de la siguiente manera: 

- 200 indicadores técnicos 

- 40 variables de volatilidad 

- 30 variables de volumen 

- 20 variables de microestructura 

- 10 variables de sentimiento 

Al analizar la matriz de correlaciones y calcular su rango, se obtiene el siguiente resultado: 

**==> picture [90 x 11] intentionally omitted <==**

Esto implica que, a pesar de contar con 300 variables, solo 8 dimensiones contienen información verdaderamente independiente. Las restantes variables son redundantes, muchas de ellas son combinaciones lineales de otras, y en conjunto pueden generar problemas de multicolinealidad. Además, muchas de estas variables son transformaciones derivadas del mismo precio u otra fuente, aportando principalmente ruido y poca información adicional útil para la modelización. 

## **1.1.2 Arquitectura conceptual del flujo de datos en los mercados financieros.** 

En los mercados financieros modernos, el análisis predictivo basado en tendencias depende directamente de la capacidad de gestionar las Tres V del Big Data: volumen, velocidad y variedad. El volumen creciente de transacciones, la velocidad extrema con la que se generan los eventos del mercado y la variedad cada vez mayor de fuentes, precios, volúmenes, libros de órdenes, noticias, sentimiento y datos alternativos obligan a diseñar arquitecturas capaces de capturar, procesar y 

transformar información heterogénea en señales predictivas robustas. En este contexto, la calidad del modelo no depende únicamente de la técnica empleada, sino de la capacidad del sistema para integrar datos diversos, limpiarlos, alinearlos temporalmente y extraer de ellos la estructura informativa relevante para anticipar la dirección del precio. 

La Figura 1.1 ilustra precisamente esta lógica mediante tres capas funcionales que representan el flujo completo de un sistema predictivo basado en Big Data. La primera capa, adquisición y fuentes de datos, integra información proveniente de mercados tradicionales (precios, volúmenes, microestructura), datos alternativos (redes sociales, imágenes satelitales, sentimiento) y fundamentales económicos. La segunda capa, procesamiento y análisis en tiempo real, aplica técnicas de limpieza, normalización, análisis multivariante y reducción de dimensionalidad para transformar datos brutos en representaciones informativas aptas para modelización. Finalmente, la tercera capa, decisión y retroalimentación, utiliza modelos cuantitativos para generar señales de trading accionables, evaluarlas continuamente y retroalimentar el sistema, cerrando el ciclo de aprendizaje y optimización. 

Esta estructura refleja cómo, en un entorno dominado por Big Data, la ventaja competitiva no proviene solo del modelo predictivo, sino de la capacidad de toda la arquitectura para convertir datos masivos, veloces y variados en decisiones precisas y oportunas. 

Figura 1.1 Arquitectura conceptual del flujo de datos en los mercados financieros 

```{figure} 01_big_data_images/4._Flujo_de_datos_Mercados.png
---
width: 90%
name: fig-flujo-datos
align: center
---
Arquitectura conceptual del flujo de datos en los mercados financieros.
```

## **a. Capa de adquisición y fuentes de datos (Volumen y Variedad)** 

Esta primera parte de la imagen, situada en el extremo inicial del flujo, representa la entrada masiva y heterogénea de información: cotizaciones intradías, libros de órdenes, noticias, redes sociales, indicadores macroeconómicos y datos alternativos. Aquí se materializan las dos primeras V: 

- **Volumen** , por la magnitud de observaciones generadas cada segundo. 

- **Variedad** , por la coexistencia de datos estructurados (precios, volúmenes) y no estructurados (texto, sentimiento, imágenes satelitales en casos especializados). 

En este contexto, el sistema financiero moderno ya no depende solo de datos de mercado, sino de un ecosistema informacional mucho más amplio que requiere integración semántica y limpieza automatizada. 

## **b. Capa de procesamiento y análisis en tiempo real (Velocidad)** 

En el centro del diagrama se observa el núcleo de procesamiento, donde los flujos de datos se transforman mediante streaming analytics, machine learning y algoritmos predictivos. Aquí se enfatiza la Velocidad, pues los sistemas deben operar con latencias de milisegundos para permitir decisiones automáticas en trading algorítmico o gestión de riesgos. 

La eficiencia del sistema depende de la capacidad de procesar y reaccionar en tiempo real, lo que convierte la velocidad en un principio de diseño, no solo una característica técnica. 

## c **. Capa de decisión y retroalimentación (Integración de las tres V)** 

En la parte final del flujo, donde los resultados analíticos se traducen en decisiones como órdenes de compra/venta, alertas de riesgo y ajustes de portafolio, se integran las tres V y por tanto, el sistema se vuelve data-driven porque: 

- El volumen de datos alimenta los modelos predictivos. 

- La variedad de los datos permite obtener una visión multidimensional del mercado. 

- La velocidad garantiza que las decisiones sean oportunas y competitivas. 

Esta última fase cierra el ciclo, evidenciando por una parte cual ha sido la transición de los sistemas financieros tradicionales, basados en análisis retrospectivo, hacia entornos predictivos y adaptativos, donde la información fluye de manera continua y retroalimenta los modelos. 

## **1.2. Acción del Precio como Núcleo Predictivo** 

La acción del precio constituye el punto de partida estratégico y metodológico para comprender mejor la dinámica subyacente del mercado. En lugar de depender de señales externas, modelos opacos o indicadores derivados que diluyen la estructura real del movimiento, este enfoque hace que el análisis se centre en lo que el mercado verdaderamente revela: la interacción entre precios, volumen, divergencias internas y el contexto de la tendencia dominante. 

A continuación, se describen los cinco grupos de variables que conforman este núcleo predictivo, cada uno capturando un aspecto esencial del comportamiento del mercado antes, durante y después de un cambio de tendencia. 

## **1.2.1. Variables primarias** 

Las variables primarias representan el corazón cuantitativo del análisis. Son medidas directas, no transformadas y altamente interpretables que describen el comportamiento del precio y del volumen en las 18 velas previas al instante ET (punto de inflexión). Su función es capturar la microestructura del mercado justo antes de que se produzca un giro direccional. 

Figura 1.2.1. Variables Primarias 

```{figure} 01_big_data_images/6._Variables_primarias.png
---
width: 90%
name: fig-variables-primarias
align: center
---
Variables Primarias.
```

Esta imagen muestra la arquitectura de las variables primarias útiles para capturar la información relevante con la microestructura del mercado. El análisis de las medidas demostró que con un número de periodos de 18 periodos previos al punto de inflexión ET, permite obtener resultados satisfactorios. 

Esta imagen muestra la arquitectura de las variables primarias útiles para capturar la información relevante con la microestructura del mercado. Mediante un análisis de medidas exhaustivo, se demostró que 18 periodos previos al punto de inflexión ET permite obtener medidas con resultados significativos y satisfactorios en la comprensión de la dinámica del mercado. Sin embargo, el análisis de las medidas con este número de periodos mostró que la arquitectura de variables primarias se correlaciona significativamente con la información relevante de la microestructura del mercado, lo que sugiere que esta arquitectura es efectiva para capturar los patrones y tendencias clave del mercado. 

- Variables basadas en el precio de cierre 

Estas variables cuantifican la forma en que el precio se desplaza, oscila y se dispersa en el corto plazo, Incluyen medidas como: 

- El spread del precio de cierre, 

- La media de los rendimientos, 

- La dispersión de dichos rendimientos. 

Su propósito es describir la intensidad, estabilidad y direccionalidad del movimiento reciente del precio, permitiendo identificar si el mercado se encuentra en expansión, contracción o transición. 

## **Rendimiento logarítmico (** 𝑹𝒊) 

El retorno logarítmico de un activo financiero es la variación logarítmica entre dos precios de cierre consecutivos, lo que permite medir el cambio relativo del precio en un período específico. Esta medida estadística es particularmente útil en el análisis de finanzas, ya que proporciona información sobre la tendencia y la volatilidad del precio de un activo. De acuerdo con (Campbell, 1997) el retorno logarítmico se obtiene así: 

**==> picture [218 x 24] intentionally omitted <==**

## Donde: 

𝒄𝒑𝒊= precio de cierre registrado por un activo financiero en el periodo i 𝒄𝒑𝒊−𝟏= precio de cierre registrado por un activo financiero en el periodo i-1 

## _**Ejemplo:**_ 

Suponiendo que el tipo de cambio euro/dólar tiene los siguientes precios de cierre (𝑐𝑝𝑖) para los días 𝑐𝑝𝑖−1= 1.1528 y 𝑐𝑝𝑖= 1.1568, aplicando la fórmula del retorno logarítmico: 

**==> picture [329 x 25] intentionally omitted <==**

El valor de 0.00346 representa el retorno logarítmico en términos continuos obtenido entre dos períodos. En porcentaje, este rendimiento equivale aproximadamente a un 0.346%, reflejando la tasa de cambio relativa del activo en ese intervalo. 

- Variables basadas en el volumen 

En los mercados financieros, el volumen actúa como un indicador de la actividad y el interés del mercado, funcionando como el “pulso” del mismo. Sin embargo, en el trading de divisas (Forex), el volumen real de transacciones no es observable en tiempo real debido a su naturaleza OTC (Over The Counter). Por ello, se emplean variables proxy, como el tick volume, que representa el número de cambios de precio en un periodo determinado y que ha demostrado ser un indicador útil de la actividad del mercado. En este contexto, estas variables capturan aspectos como: 

- La amplitud del volumen proxy negociado, 

- La variación promedio de dicho volumen, 

- La dispersión o volatilidad de estas variaciones. 

El análisis del volumen, incluso en su forma proxy, ayuda a confirmar o contradecir la acción del precio. Un movimiento de precio sin un aumento en el volumen proxy puede carecer de credibilidad, mientras que un movimiento acompañado de un incremento en el volumen suele anticipar la continuidad o una ruptura en la tendencia. Estas variables permiten evaluar la fuerza interna del movimiento y la intensidad del interés en el mercado. 

## **Volatilidad del volumen (** 𝜎𝑣 **):** 

La volatilidad del volumen es una medida estadística que cuantifica la dispersión, variabilidad o inestabilidad del volumen negociado (o del volumen proxy, como el tick volume) alrededor de su 

media en un periodo determinado. Refleja la intensidad y la irregularidad de la actividad del mercado, permitiendo identificar fases de acumulación, distribución, ruptura o agotamiento de tendencia. De acuerdo con (Hasbrouck, 2007), matemáticamente, corresponde a la desviación estándar del volumen en una ventana temporal especificada. 

**==> picture [132 x 50] intentionally omitted <==**

Donde: 

𝑣𝑖=Volumen o tick volumen en el periodo i 

𝑣̅= Volumen promedio 

𝑛 = Número de observaciones 

Por otra parte, en el análisis cuantitativo y en la microestructura de mercado, la volatilidad del volumen se debe interpretar de manera relativa. Esto se debe a que el volumen y especialmente el tick volume en mercados OTC como Forex presenta distribuciones altamente variables según el activo, el régimen de volatilidad y la hora del día. 

En este contexto, la literatura científica establece que los niveles de actividad deben evaluarse mediante umbrales basados en los percentiles, derivados de la distribución histórica del propio activo. Esta metodología está respaldada por trabajos fundamentales como Karpoff (1987), Hasbrouck (2007) y Campbell, Lo & MacKinlay (1997), quienes demuestran que la intensidad informacional del mercado se manifiesta en incrementos relativos de la variabilidad del volumen, no en valores absolutos. 

La siguiente tabla resume los umbrales universalmente aceptados para clasificar la volatilidad del volumen en Big Data financiero. 

Tabla 1. Umbrales según percentiles de volatilidad del volumen 

|Nivel de<br>volatilidad|Criterio<br>matemático|Interpretación|
|---|---|---|
|Baja|𝜎𝑣< P25|**Actividad reducida**; bajo interés del mercado; movimientos de<br>preciopoco fiables.|
|Normal|P25 ≤𝜎𝑣≤ P75|**Actividad**<br>**típica**<br>**del**<br>**mercado**;<br>condiciones<br>estables;<br>movimientos con credibilidad moderada.|
|Alta|𝜎𝑣> P75|**Aumento significativo de la actividad**; mayor intensidad<br>informacional; probabilidad elevada de ruptura o continuación<br>de tendencia.|
|Extremadamente<br>Alta<br>(evento<br>informacional)|𝜎𝑣> P90|**Actividad excepcional**; entrada de institucionales; anuncios<br>macro; alta probabilidad de movimientos impulsivos.|



Es importante tener en cuenta que, un aumento brusco en la volatilidad del volumen (𝜎𝑣) suele anticipar rupturas de soporte/resistencia, cambios de tendencia, movimientos impulsivos, entrada 

de participantes institucionales, entre otros aspectos clave en la negociación de instrumentos financieros. 

## _**Ejemplo:**_ 

Para ilustrar cómo se evalúa la volatilidad del volumen en Big Data financiero, considere el tick volume del par EUR/USD en velas de 5 minutos. Estos valores representan la actividad del mercado en cinco intervalos consecutivos, tal como se resume en la tabla 1. 

Tabla 1. Tick Volume del par EUR/USD (5 minutos) 

|**Minuto**|**Tick Volume**|
|---|---|
|1|980|
|2|1200|
|3|1500|
|4|1100|
|5|2100|



Al calcular el valor medio del tick volumen, 𝑣̅= 1376 ticks y la volatilidad del volumen experimentada durante los 5 minutos, 𝜎𝑣 = 448.2 ticks. La volatilidad del volumen del EUR/USD es 448.2 ticks. 

Ahora suponga que, a partir de una ventana histórica de 2.000 observaciones del EUR/USD, se obtienen los siguientes percentiles: 

Tabla 2. Percentiles históricos del par EUR/USD 

|Percentil|Valor<br>(ticks)|Volatilidad|Interpretación operativa|
|---|---|---|---|
|P25|180|Baja|Actividad reducida; bajo interés del mercado;<br>movimientos depreciopoco fiables.|
|P50|260|Normal (media)|Comportamiento típico del mercado; condiciones<br>estables;credibilidad moderada.|
|**P75**|**410**|**Alta**|Aumento significativo de la actividad; mayor intensidad<br>informacional; probabilidad elevada de ruptura o<br>continuación de tendencia.|
|P90|580|Extremadamente Alta<br>(evento informacional)|Actividad excepcional; entrada de institucionales;<br>anuncios<br>macro;<br>movimientos<br>impulsivos<br>y<br>direccionales.|



Al hacer una Interpretación operativa en función de los percentiles anteriores y una volatilidad del volumen de 448.2 ticks, ubicada por encima del percentil 75, indica: 

- Incremento significativo en la actividad del mercado, 

- Mayor intensidad informacional, 

- Probabilidad elevada de ruptura o continuación de tendencia, 

- Posible entrada de participantes institucionales. 

En la construcción de modelos predictivos, este nivel de actividad suele reforzar las señales de precio, anticipar movimientos direccionales y filtrar señales falsas cuando el volumen es bajo. 

- Variables que miden desacoplamientos entre precio, volumen e indicadores 

En el análisis de mercado, existen fenómenos llamados desacoplamientos, donde los diferentes componentes del mercado muestran comportamientos divergentes. Estos desacoplamientos pueden ser señales críticas en la formación de puntos de inflexión, es decir, cambios en la tendencia general del mercado. A continuación, se presentan algunas variables que miden estos desacoplamientos: 

- Discrepancias entre precio y volumen 

Cuando el precio sube o baja sin que el volumen de negociación lo acompañe, o viceversa, puede ser un indicador de que el mercado está experimentando un desacoplamiento. Esto puede ser una señal de que la tendencia está cambiando. 

- Discrepancias entre indicadores tecnológicos 

La divergencia entre diferentes indicadores técnicos, por ejemplo, como el índice de fuerza relativa (RSI), la media móvil simple (MMA) y la media móvil exponencial (EMA), también puede ser un indicador de desacoplamiento. Cuando estos indicadores muestran resultados divergentes, puede ser un signo de que el mercado está experimentando una fase de transición. 

- Discrepancias entre precio y otros indicadores de mercado 

La divergencia entre el precio de un activo financiero y otros indicadores de mercado, como la actividad de los compradores y vendedores, la posición de los traders y la economía general, también puede ser un indicador de desacoplamiento. Esto puede ser una señal de que el mercado está experimentando un cambio en la tendencia. 

## **Medida de divergencia normalizada (D)** 

En el análisis cuantitativo de mercados y en el ámbito del Big Data financiero, una de las herramientas más robustas para detectar desacoplamientos entre precio, volumen e indicadores técnicos es la divergencia normalizada. De acuerdo con Campbell (1997), esta medida permite identificar cuándo dos variables que normalmente evolucionan de forma coherente comienzan a mostrar comportamientos divergentes, lo cual suele anticipar puntos de inflexión, cambios de tendencia o rupturas estructurales en el mercado. 

La divergencia normalizada se define como: 

**==> picture [94 x 27] intentionally omitted <==**

## Donde: 

𝐴𝑖, 𝐵𝑖 = series que se comparan (por ejemplo, precio vs. volumen, precio vs. RSI, RSI vs. EMA), 𝜎𝐴−𝐵  = desviación estándar muestral histórica de la diferencia entre ambas series. 

Esta normalización es fundamental porque: elimina el efecto de las unidades distintas, permite comparar desacoplamientos entre múltiples variables, convierte la diferencia en una magnitud 

estadísticamente interpretable y permite detectar eventos significativos cuando la divergencia supera 1.5, 2 o más desviaciones estándar. 

Al analizar los patrones de desacoplamiento en la información financiera, es importante establecer umbrales para determinar la relevancia predictiva de los resultados. En términos operativos, estos umbrales pueden ser clasificados de la siguiente manera: 

- |D| < 1 → desacoplamiento normal, sin relevancia predictiva, 

- |D| > 2 → evento estadísticamente significativo, 

- |D| > 3 → fuerte señal de transición o punto de inflexión. 

Esta métrica es especialmente útil en Forex, donde el volumen real no es observable y se trabaja con proxies como el tick volume. La divergencia normalizada permite evaluar si el precio, el volumen y los indicadores técnicos están alineados o si existe un desacoplamiento que anticipe un cambio de régimen. 

## _**Ejemplo:**_ 

A continuación, se presenta un ejemplo basado en datos del par EUR/USD en velas de 1 hora. El ejemplo incluye: precios de cierre, valores del RSI (14), cálculo de variaciones, divergencia normalizada y la interpretación operativa. 

Tabla 3. Series históricas del precio de cierre y el valor RSI (14) del par EUR/USD 

|Periodo|Precio Cierre(EUR/USD)|RSI(14)|
|---|---|---|
|𝑖−4|1.0830|58|
|𝑖−3|1.0845|55|
|𝑖−2|1.0860|52|
|𝑖−1|1.0875|49|
|𝑖|1.0900|44|



En la tabla anterior se observa un claro desacoplamiento en el mercado, donde el precio alcanza un aumento de 70 puntos desde 1.0830 hasta 1.0900, mientras que el RSI cae drásticamente de 58 a 44 puntos. Esta disminución en la fuerza interna del movimiento, a pesar del aumento en el precio, es un indicio de un desacoplamiento clásico, donde el precio y la fuerza interna no están alineados. En la Tabla 4 se resume el procedimiento utilizado para el calculo de la divergencia normalizada (D): 

Tabla 4. Divergencia normalizada (D) 

|Periodo|Precio cierre|RSI(14)|∆ P|∆ RSI|∆𝑃𝑖−∆𝑅𝑆𝐼𝑖|𝐷𝑃,   𝑅𝑆𝐼(𝑖)|
|---|---|---|---|---|---|---|
|𝑖−4|1.0830|58|||||
|𝑖−3|1.0845|55|0.0014|-0.0531|0.054|2.07|
|𝑖−2|1.0860|52|0.0014|-0.0561|0.057|2.19|
|𝑖−1|1.0875|49|0.0014|-0.0594|0.061|2.31|
|𝑖|1.0900|44|0.0023|-0.1076|0.110|4.18|
|||||𝜎∆𝐴−∆𝐵|**0.026**||



De acuerdo con los resultados obtenidos, en la última columna se observan los valores de la divergencia normalizada 𝐷𝑃,   𝑅𝑆𝐼(𝑖). En las columnas ΔP y ΔRSI, se destaca el desacoplamiento en todos los tramos, ya que mientras el precio de cierre sube, los valores de RSI bajan. Esto se refleja en 𝐷𝑃,   𝑅𝑆𝐼(𝑖) > 2. Es importante destacar que el último tramo es claramente crítico, ya que el precio acelera al alza, el RSI se desploma y la divergencia normalizada alcanza un valor excepcional de 4.18, lo que lo convierte en un evento muy raro. 

En términos de la lógica de los puntos de inflexión, los tres primeros tramos sugieren un desacoplamiento progresivo, mientras que el último tramo presenta una divergencia significativa en la que se puede intuir la ocurrencia de un punto de inflexión que merece ser analizado más a fondo. 

## **1.2.2. Problemas estructurales en la predicción basada en la acción del precio.** 

La literatura contemporánea sobre predicción del movimiento direccional de los precios de los activos financieros ha logrado avances significativos en términos de capacidad computacional. Sin embargo, estos avances no han sido acompañados de una comprensión profunda de los mecanismos que rigen la acción del precio. En el contexto de la construcción de modelos predictivos, existen un conjunto de problemas estructurales, recurrentes y ampliamente documentados, que limitan la eficacia de los modelos existentes. A continuación, se presenta un breve resumen de los principales problemas que actualmente influyen en la construcción de modelos predictivos, como se muestra en la siguiente figura. 

Figura 1.2.2. Problemas estructurales en la formulación de modelos predictivos. 

```{figure} 01_big_data_images/7._Problemas_Estructurales.png
---
width: 90%
name: fig-problemas-estructurales
align: center
---
Problemas estructurales en la formulación de modelos predictivos.
```

## **1. Falta de interpretabilidad en los modelos predictivos** 

Uno de los problemas más importantes que actualmente influye en la construcción de modelos predictivos es la incapacidad de los modelos dominantes para explicar por qué predicen lo que predicen. Técnicas como LSTM, SVM, redes neuronales profundas o modelos híbridos consiguen altos niveles de precisión en la predicción, pero este éxito se logra a costa de la comprensión de los 

mecanismos subyacentes que generan las predicciones. En un entorno financiero, donde las decisiones deben ser justificables, esta opacidad es inaceptable. 

La consecuencia de este problema es doble: por una parte, el analista no puede comprender qué variables impulsan la señal o determinan la dirección del precio y, por otra parte, el modelo no puede ser auditado ni validado en términos económicos. 

Este vacío metodológico se constituye en el punto de partida para la estructuración y formulación de una metodología que permita construir modelos predictivos parsimoniosos y que por tanto se convierte en un problema abierto a la investigación. 

## **2. Complejidad excesiva y naturaleza “caja negra”** 

La literatura ha evolucionado hacia modelos cada vez más complejos, con arquitecturas profundas, hiperparámetros difíciles de calibrar y comportamientos altamente no lineales. Sin embargo, esta complejidad no se traduce en una mejora proporcional del rendimiento, y sí introduce varios problemas, como: 

- Sensibilidad extrema a la estructura de los datos 

- Dependencia de configuraciones específicas 

- Dificultad para replicar resultados 

En este contexto, los resultados de las últimas investigaciones sugieren que la complejidad excesiva y la naturaleza 'caja negra' de estos modelos han desplazado la comprensión del fenómeno subyacente, limitando su capacidad de generalización y mejora del rendimiento en diferentes escenarios. 

## **3. Sobreajuste y baja capacidad de generalización** 

Los modelos de aprendizaje automático y otros modelos estadísticos con frecuencia caen en la trampa de la captura de patrones espurios presentes en los datos históricos. Esta limitación los hace incapaces de reproducirse con precisión en escenarios futuros, particularmente en el modelamiento de los precios de los activos financieros, donde: 

- La señal de tendencia subyacente está frecuentemente oculta por el ruido y la volatilidad de los precios en el mercado. 

- Las distribuciones de los precios cambian con el tiempo, lo que dificulta la generalización y el desarrollo de modelos robustos. 

- La complejidad sin parsimonia puede conducir a modelos frágiles y propensos al sobreajuste, lo que reduce su capacidad predictiva. 

Para abordar este desafío, es necesario desarrollar estrategias y técnicas innovadoras que permitan a los modelos ser más flexibles y adaptables a cambios en las distribuciones y en las relaciones entre variables, y que mitiguen el problema del sobreajuste, mejorando así la precisión y la confiabilidad de los modelos predictivos. 

## **4. Inestabilidad paramétrica ante cambios estructurales del mercado** 

Al entender el mercado financiero como un entorno complejo y dinámico, caracterizado por cambios estructurales permanentes en la volatilidad, las correlaciones y los regímenes de precios, los modelos predictivos además de ser precisos, también deben ser estables y capaces de adaptarse a los cambios de régimen en el mercado. Sin embargo, esta inestabilidad es un desafío para muchos modelos tradicionales, que pueden ser sensibles a cambios en los parámetros del mercado. Algunos de los problemas asociados con la inestabilidad paramétrica en los modelos financieros incluyen: 

- Sensibilidad a cambios en la volatilidad del mercado, lo que puede afectar la precisión del modelo. 

- Cambios en las correlaciones entre los activos, lo que puede generar resultados incorrectos. 

- Cambios en el régimen del mercado, lo que puede provocar desviaciones significativas. 

En este contexto de operación, la inestabilidad de los modelos puede tener consecuencias significativas que pueden llevar a varios problemas como la toma de decisiones incorrectas que pueden resultar en pérdidas financieras, debilitar la confianza en los modelos y dificultar la toma de decisiones informadas. Para abordar estos desafíos, es necesario desarrollar modelos más flexibles que puedan adaptarse a los cambios en el mercado. 

## **5. Distribuciones no normales en los retornos del precio** 

Es bien sabido que los retornos de los instrumentos financieros, especialmente aquellos generados por la negociación del tipo de cambio EUR/USD, presentan: 

- Asimetría marcada, 

- Leptocurtosis extrema, 

- Colas pesadas, 

- Alta concentración de valores pequeños. 

Estas características violan los supuestos de normalidad que sustentan muchos métodos estadísticos tradicionales. Ignorar la verificación de estos supuestos dificulta la utilización de métodos estadísticos multivariantes para la construcción de modelos predictivos y puede llevar a conclusiones erróneas y modelos mal especificados. 

## **6. Selección deficiente de variables y exceso de indicadores.** 

Uno de los mayores desafíos en la construcción de modelos predictivos para pronosticar la dirección o tendencia del precio de los activos es identificar las variables que realmente tienen un impacto causal y discriminante en el movimiento del precio (relevancia). La tendencia común de adoptar el paradigma de que "más variables es mejor" puede conducir a problemas de multicolinealidad y la formación de modelos sobreajustados y difíciles de interpretar, donde la inclusión indiscriminada de indicadores técnicos, financieros o derivados del análisis fundamental no garantiza una mejor predicción. 

El uso excesivo de variables suele sacrificar la interpretabilidad y la trazabilidad del modelo, además de requerir técnicas de reducción de dimensionalidad como análisis de componentes principales o 

análisis factorial, que transforman las variables originales en componentes o factores, pero que dificultan entender qué factores específicos conducen a la predicción. Por tanto, la clave está en identificar y seleccionar variables con alto poder discriminativo y causal, aquellas que tengan la capacidad de diferenciar claramente cuándo un activo tenderá a subir o bajar. La correcta selección de estas variables relevantes permite construir modelos no solo precisos, sino también interpretables y útiles para la toma de decisiones, evitando la dependencia excesiva en un volumen desmedido de indicadores que, en última instancia, pueden disminuir la capacidad predictiva y la claridad del modelo. 

## **7. Ausencia de análisis del contexto previo a los cambios de tendencia** 

Muchos estudios en el ámbito financiero se enfocan en predecir retornos, clasificar movimientos o detectar patrones, pero generalmente omiten analizar en profundidad los momentos que preceden a los puntos de inflexión en los precios. Estos momentos, en los que se concentra información valiosa sobre posibles cambios de tendencia, suelen ser subestimados o pasados por alto, limitando la comprensión completa de la dinámica del mercado. 

Este vacío metodológico puede dificultar la identificación temprana de cambios relevantes y reducir la capacidad de anticipar movimientos significativos, lo que representa una limitación importante para la elaboración de modelos predictivos más robustos y explicativos. Al ignorar los momentos previos a los puntos de inflexión, donde se concentra la información más valiosa, implícitamente se limita la comprensión de la dinámica real del mercado. En este contexto, construir un modelo predictivo sin la consideración de un punto de referencia en el mercado, que sirva como base para aplicar el conocimiento existente, puede limitar significativamente su precisión y utilidad, dificultando la detección de patrones relevantes y la anticipación de cambios futuros. 

## **8. Dependencia excesiva de datos exógenos o Análisis de Sentimiento** 

La acción del precio, si se analiza de manera adecuada, puede proporcionar información valiosa para construir modelos predictivos efectivos, reduciendo en cierta medida la dependencia de datos exógenos. Desde la perspectiva de la hipótesis de los mercados eficientes en su forma más fuerte, toda la información relevante ya está reflejada en el precio, lo que implica que los movimientos del mercado reflejan de manera inmediata las expectativas y valoraciones de los inversores. 

En este contexto, el análisis técnico, enfocado en variables que miden la acción del precio, como medias móviles, niveles de soporte y resistencia, patrones de velas, indicadores de momentum y volumen, resulta siendo una herramienta útil para identificar tendencias y puntos de inflexión en el mercado. Sin embargo, es importante reconocer que, en la práctica, variables externas como noticias, eventos macroeconómicos o políticos pueden influir en el mercado y afectar la estabilidad y la predictibilidad de los modelos basados únicamente en la acción del precio. 

Aunque estos eventos pueden introducir ruido, en muchas ocasiones, la acción del precio refleja, en tiempo real, la suma de las expectativas y reacciones del mercado, constituyendo un indicador valioso para la toma de decisiones, siempre complementado con un análisis contextual adecuado. 

## **9. Falta de modelos parsimoniosos, robustos y estables** 

La literatura actual carece de modelos parsimoniosos que cumplan simultáneamente con las siguientes características: 

- Interpretable: fácil de entender y explicar cómo funcionan las relaciones entre las variables. 

- Preciso: capaz de hacer predicciones precisas, basadas en los datos de entrada. 

- Generalizable: capaz de predecir con precisión en diferentes contextos y escenarios con nuevos datos o escenarios, sin necesidad de ajustes adicionales. 

Este enfoque debe estar centrado en la selección estructural de variables, lo que significa que las variables predictoras se identifican y seleccionan según las especificaciones del método utilizado. Por tanto, el propósito del proceso de selección de variables está en mantener la causalidad, trazabilidad e interpretabilidad de los valores estimados en función de las variables predictoras que mejor explican y modelan el fenómeno objeto de simulación y predicción. 

## **Síntesis final** 

Los problemas identificados forman un ecosistema de limitaciones que ha impedido que la predicción basada en la acción del precio avance hacia modelos explicativos, robustos y científicamente sólidos. Por tanto, la solución en cuanto a la construcción de modelos predictivos no está en aumentar su complejidad, sino en comprender la estructura del mercado, seleccionando las variables relevantes que permiten construir modelos parsimoniosos. 

## **TIP DIDÁCTICO** 

En la construcción de modelos predictivos de la dirección o tendencia del precio del activo, es importante evitar incluir variables derivadas del precio sin un análisis previo de su capacidad discriminativa, de multicolinealidad, independencia y estructura multivariante. 

## **Bibliografía.** 

- Gandomi, A., & Haider, M. (2015). Beyond the hype: Big data concepts, methods, and analytics. International Journal of Information Management, 35(2), 137–144. 

- Chen, M., Mao, S., & Liu, Y. (2014). Big Data: A Survey. Mobile Networks and Applications, 19, 171–209. 

- Jolliffe, I. T., & Cadima, J. (2016). Principal component analysis: a review and recent developments.  Philosophical Transactions of the Royal Society A. 

- Campbell, J. Y., Lo, A. W., & MacKinlay, A. C. (1997). The Econometrics of Financial Markets. Princeton University Press. 

- Hasbrouck, J. (2007). Empirical Market Microstructure. Oxford University Press. 

- Karpoff (1987). The Relation Between Price Changes and Trading Volume. Journal of Financial and Quantitative Analysis 



---

## Imágenes extraídas


```{image} 01_big_data_images/page7_img1.jpeg
:alt: Imagen extraída del PDF
:width: 80%
:align: center
```


```{image} 01_big_data_images/page9_img1.jpeg
:alt: Imagen extraída del PDF
:width: 80%
:align: center
```


```{image} 01_big_data_images/page15_img1.jpeg
:alt: Imagen extraída del PDF
:width: 80%
:align: center
```
