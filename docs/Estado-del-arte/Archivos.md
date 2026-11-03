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
