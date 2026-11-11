## Relevancia máxima
 1. Evaluation of spontaneous fermentation impact on the physicochemical properties and sensory profile of green and roasted arabica coffee by digital technologies

```mermaid
mindmap
  root((Fermentación y aroma medidos con e-nose, NIR y ANN))
    q{{Pregunta de investigación}}
      ¿La fermentación húmeda cambia volátiles y perfil sensorial?
      ¿NIR y e-nose pueden estimar volátiles e intensidades sensoriales?
    d{{Diseño experimental}}
      2 fincas australianas
        Mountain Top Estate
        Kahawa Estate
      Fermentado vs. no fermentado
      4 niveles: verde, claro, medio y oscuro
      16 combinaciones finca × fermentación × tostado
    i{{Instrumentación}}
      E-nose de bajo costo
      Espectroscopía NIR
      HS-SPME-GC-MS como referencia química
      Análisis descriptivo cuantitativo QDA
    m{{Modelado}}
      Regresión con redes neuronales artificiales
      Entradas: absorbancias NIR o señales de la e-nose
      Salidas: áreas de pico GC-MS e intensidades sensoriales
      4 modelos independientes
    h{{Hallazgos}}
      Verde fermentado: notas a heno
      Tostado fermentado: más chocolate amargo, tostado, mantequilla y crema
      Metilpirazina y etil-metilpirazinas separan fermentado de no fermentado
      Modelos de volátiles: R = 0.98 y R = 0.87
      Modelos sensoriales: R = 0.91
    l{{Puntos a revisar}}
      Pocas unidades independientes para una ANN
      Reporta R, no R² ni RMSEP
      Validación externa por confirmar en texto completo
```
4\. **Detection and Differentiation of Volatile Compound Profiles in Roasted Coffee Arabica Beans from Different Countries Using an Electronic Nose and GC-MS**

Gancarz y colaboradores (2020) compararon cafés arábica de Brasil, Etiopía, Guatemala, Costa Rica y Perú, tostados bajo las mismas condiciones. Contrastaron las respuestas de los ocho sensores de la Agrinose con los perfiles de volátiles obtenidos por GC-MS. El análisis de componentes principales separó especialmente la muestra brasileña de las de Etiopía, Guatemala y Costa Rica. La cromatografía encontró niveles elevados de piridina en Brasil y Perú. Para FONFIVE, el estudio aporta un ejemplo de cómo contrastar la huella de la nariz electrónica con una referencia química independiente. [Artículo original](https://doi.org/10.3390/s20072124)

```mermaid
mindmap
  root((Café arábica tostado y perfil volátil))
    Cinco orígenes con el mismo régimen de tostado
    Agrinose con ocho sensores y GC-MS
    Separación destacada de la muestra brasileña
    Piridina elevada en Brasil y Perú
```

## Relevancia muy alta
5. Electronic Nose and Gas Chromatograph Devices for the Evaluation of the Sensory Quality of Green Coffee Beans

```mermaid
mindmap
  root((Calidad del grano verde: e-nose frente a GC-MS))
    q{{Pregunta de investigación}}
      ¿Las calidades de café verde se distinguen por sus COV?
      ¿Una e-nose puede clasificar calidad sin tostar ni preparar bebida?
    mat{{Material}}
      Coffea arabica en grano verde fresco
      Clases de calidad asignadas por panel de cata
    tec{{Técnicas}}
      GC-MS para perfil de compuestos volátiles
      Nariz electrónica
      Panel sensorial con atributos positivos y negativos
    qm{{Quimiometría}}
      PCA exploratorio
      PLS-DA para clasificar calidad
      PLS para cuantificar aroma frutal
    hq{{Hallazgos químicos}}
      Alta calidad: frutal, herbal y dulce
        Más alcoholes y compuestos aromáticos
        Feniletil alcohol, nonanal, 2-metilpropanoato de octilo
      Baja calidad: tostado, ahumado y fermentación anormal
        Más ácidos carboxílicos, pirazinas y piridinas
        Piridina, ácido octanoico, dimetilsulfuro
    he{{Desempeño de la e-nose}}
      PLS-DA explica 96.9 % de la varianza total
      Aroma frutal predicho con R² de predicción = 0.88
      Dispositivo no destructivo y de bajo costo
    l{{Puntos a revisar}}
      Grano verde: no evalúa la taza
      Varianza explicada no equivale a exactitud de clasificación
      Número de lotes y tipo de validación por confirmar
```

8\. **Effectiveness of an E-Nose Based on Metal Oxide Semiconductor Sensors for Coffee Quality Assessment**

Mutz y colaboradores (2025) construyeron una nariz electrónica con 12 sensores MOS, una cámara de medición y un Arduino Mega. Evaluaron la clasificación por especie, grado de tostado y caducidad. El modelo LS-SVM clasificó correctamente todas las muestras de prueba en las tres tareas. Los cafés caducados llevaban alrededor de dos años fuera de fecha, por lo que ese resultado corresponde a grupos con una diferencia marcada. El montaje sirve como referencia para integrar los sensores, la cámara y la adquisición de señales de FONFIVE. [Artículo original](https://doi.org/10.3390/chemosensors13010023)

```mermaid
mindmap
  root((Matriz MOS para clasificar café))
    Doce sensores MOS y Arduino Mega
    Especie, grado de tostado y caducidad
    LS-SVM clasificó todas las muestras de prueba
    Cafés vencidos desde hacía unos dos años
```

## Relevancia alta
9. Electronic Prediction of Chemical Contaminants in Aroma of Brewed Roasted Coffee and Quantification of Acrylamide Levels

```mermaid
mindmap
  root((E-nose como predictor indirecto de contaminantes térmicos))
    q{{Pregunta de investigación}}
      ¿La e-nose puede estimar acrilamida y 5-HMF en espresso?
    d{{Diseño experimental}}
      Granos frescos con distintos tratamientos térmicos
      Análisis sobre la bebida espresso
    me{{Mediciones}}
      Perfil de compuestos volátiles
        70 compuestos en 15 familias
      Acrilamida y 5-hidroximetilfurfural
      Panel sensorial
        Positivo: olor a café y tostado
        Negativo: olor a quemado
      Señales de la e-nose
    qm{{Quimiometría}}
      PCA de la bebida
      PLS con validación cruzada y conjunto de validación
    h{{Hallazgos}}
      Familias dominantes: furanos, pirazinas, piridinas y aldehídos
      Relación lineal entre tóxicos y defecto sensorial
        Más defecto implica menos acrilamida
        Más defecto implica más 5-HMF
      Señal de la e-nose correlaciona con el defecto
      Cadena indirecta: e-nose → defecto → contaminante
    l{{Puntos a revisar}}
      La predicción depende de que se mantenga la relación defecto-contaminante
      Esa relación puede cambiar con origen, variedad o perfil de tostado
      Mide la bebida, no el grano molido
      Métricas numéricas del PLS por confirmar en texto completo
```

12\. **Accelerated storage of ground coffee: Merging of analytical techniques to assess sensitivity to oxygen and moisture exposure**

De Agostini y colaboradores (2026) almacenaron un lote de arábica molido de tueste claro en envases abiertos hasta 42 días, bajo distintas condiciones de temperatura y humedad. Compararon la nariz electrónica, HS-SPME-GC-MS y espectroscopía FT-NIR con la evaluación sensorial. El panel registró menor intensidad aromática, cuerpo y persistencia del sabor, junto con más notas oxidativas. Estos cambios coincidieron con variaciones de las señales y con la pérdida de volátiles asociados al aroma fresco. El estudio ilustra cómo relacionar las mediciones de FONFIVE con cambios perceptibles en taza. [Artículo original](https://doi.org/10.1016/j.foodres.2025.118025)

```mermaid
mindmap
  root((Deterioro del café molido))
    Arábica de tueste claro almacenado hasta 42 días
    Nariz electrónica, HS-SPME-GC-MS, FT-NIR y panel
    Menor intensidad aromática y mayor oxidación sensorial
    Alcance limitado a un lote y un grado de tostado
```

13. Electronic nose for quality control of Colombian coffee through the detection of defects in "Cup Tests"

```mermaid
mindmap
  root((A-NOSE: defectos de taza en café colombiano))
    c{{Contexto}}
      Laboratorio Almacafé en Cúcuta, Colombia
      Federación Nacional de Cafeteros
      Cata humana costosa y poco estandarizada
    hw{{Hardware}}
      Matriz de 8 sensores de óxido metálico
        Figaro serie TGS
        FIS serie SP
      Bomba de aire que arrastra volátiles a la cámara
      Ciclo de 3 etapas
        Concentración
        Medición
        Purga
    mu{{Muestreo}}
      Café arábica tipo almendra
      Molido con agua caliente a unos 60 °C
      El agua aumenta los volátiles y evita que la bomba disperse el polvo
      Muestras con y sin defecto
        Excelso como referencia
        Defecto avinagrado
    p{{Procesamiento}}
      PCA para observar agrupamientos
      MLP con retropropagación y tasa adaptativa
        10 neuronas ocultas y 1 de salida
      Validación leave-one-out
    r{{Resultados}}
      Clústeres separan café con y sin defecto
      E-nose viable como apoyo a la prueba de taza
    l{{Puntos a revisar}}
      Solo clasificación, sin puntaje continuo
      Sin referencia química GC-MS
      Leave-one-out por medición puede inflar el acierto si hay réplicas
      Efecto de humedad y deriva no descrito en el resumen
```

## Relevancia media alta
16\. **Differentiation of Chinese robusta coffees according to species, using a combined electronic nose and tongue, with the aid of chemometrics**

Dong y colaboradores (2017) analizaron 126 muestras tostadas de siete cultivares de robusta de Hainan, China. Combinaron una nariz electrónica y una lengua electrónica para diferenciar cultivares y estimar el pH, la acidez titulable y el contenido de sólidos, entre otras propiedades. La regresión por mínimos cuadrados parciales (PLSR) con datos de ambos instrumentos ofreció el mejor desempeño para estimar esos parámetros en el estudio. Para FONFIVE, es un ejemplo de calibración con mediciones de referencia y fusión de señales. La síntesis se basa en el resumen original y los extractos editoriales disponibles. [Resumen original](https://pubmed.ncbi.nlm.nih.gov/28372239/)

```mermaid
mindmap
  root((Cultivares de robusta y fusión de datos))
    126 muestras de siete cultivares de Hainan
    Nariz y lengua electrónicas
    Clasificación de cultivares y estimación fisicoquímica
    Mejor desempeño con PLSR y datos combinados
```

## Relevancia media
17. Discrimination between washed Arabica, natural Arabica and Robusta coffees by using near infrared spectroscopy, electronic nose and electronic tongue analysis

```mermaid
mindmap
  root((Enfoque holístico: NIR, e-nose y e-tongue))
    o{{Objetivo}}
      Clasificar 3 clases de café
        Robusta
        Arábica natural
        Arábica lavado
    ma{{Matrices analizadas}}
      Café verde
      Café tostado y molido
      Bebida
    t{{Técnicas}}
      Espectroscopía de infrarrojo cercano NIR
      Nariz electrónica
      Lengua electrónica
    qm{{Quimiometría}}
      PCA para correlaciones entre muestras y variables
      Selección de variables
      Análisis discriminante lineal LDA
    r{{Resultados}}
      NIR: 100 % de acierto en conjunto de prueba externo
      E-nose: 81.83 % promedio en validación cruzada
      E-tongue: 78.76 % promedio en validación cruzada
    a{{Conclusión de los autores}}
      NIR: clasificación rápida, limpia y económica
      Dispositivos electrónicos: describir aroma y sabor
    l{{Lectura crítica}}
      Las clases son especie y proceso, no calidad sensorial
      Comparación desigual: prueba externa para NIR, validación cruzada para e-nose
      Verificar si la selección de variables se hizo dentro de cada pliegue
```

## Relevancia media baja
20\. **A novel electronic nose as adaptable device to judge microbiological quality and safety in foodstuff**

Sberveglieri y colaboradores (2014) evaluaron una nariz electrónica con sensores de óxido metálico de película delgada y nanohilos. En el caso de café verde, el análisis de componentes principales distinguió cambios asociados al crecimiento de mohos desde el tercer día. El arreglo de película delgada descrito en el trabajo previo los distinguía desde el sexto. Los análisis microbiológicos y cromatográficos complementaron la interpretación. Su aporte a FONFIVE se concentra en el diseño de la matriz de sensores para detectar cambios del perfil volátil. [Artículo original](https://doi.org/10.1155/2014/529519)

```mermaid
mindmap
  root((Detección de deterioro en café verde))
    Sensores de película delgada y nanohilos
    Seguimiento de cambios por crecimiento de mohos
    Separación desde el tercer día en el ensayo
    Comparación con microbiología y cromatografía
```

## Relevancia baja
21. Investigation of non-volatile and volatile compound profiles in Arabica coffee extracts and neurophysiological effects of different chemosensory stimulation according to sex: Insights from electronic sensors, EEG, and sLORETA approaches

```mermaid
mindmap
  root((Café: química del aroma y respuesta cerebral))
    o{{Objetivo}}
      Perfil volátil y no volátil de extractos de café
      Efecto neurofisiológico de oler y de beber según el sexo
    nv{{No volátiles y sabor}}
      Cafeína y ácido clorogénico
      E-tongue: predominan acidez, amargor y salado
    v{{Volátiles y olor}}
      E-nose
      GC-MS-O: cromatografía con olfatometría
      Compuestos clave del olor
        2-furanmetanol
        Bencenoetanol
        Nonanal
        Piridina
    n{{Neurofisiología}}
      EEG con localización sLORETA
      Inhalación activa alfa rápida y beta baja
        Hombres: áreas de Brodmann 20, 21, 22, 36 y 37
        Mujeres: áreas de Brodmann 9, 27, 30, 35, 44 y 45
      Beber activa beta media igual en ambos sexos
        Áreas de Brodmann 2, 3 y 40
    a{{Aporte}}
      Referencia base sobre efectos de oler y beber café
    l{{Límites para nuestro caso}}
      Mide extractos, no grano tostado y molido
      No construye modelos de predicción de calidad
      EEG no aplica a un instrumento de laboratorio
```
