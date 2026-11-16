# Proyecto Final – Química Orgánica

# Propiedades y análisis de reacciones y obtenciones de compuestos orgánicos halogenados

Universidad Distrital Francisco José de Caldas · Ingeniería Ambiental (FAMARENA)
Proyecto N.º: 4 · Docente: Oscar Genaro García Bautista

## 📖 Descripción del proyecto

Proyecto número 4 del curso de Química Orgánica. El grupo reúne las propiedades químicas de derivados halogenados alifáticos y haluros de acilo (incluyendo monohalogenados, polihalogenados y cicloalcanos clorados, bromados y fluorados) en una tabla de datos, las analiza con gráficas en Python (Conda o Google Colab), documenta el trabajo en un informe en LaTeX y presenta los resultados en un dashboard interactivo de Power BI. El trabajo se gestiona en este repositorio, con las tareas organizadas en un GitHub Project.

## 🌍 Integrantes

| # | Nombre | Usuario de GitHub | Responsable principal de |
|---|--------|-------------------|--------------------------|
| 1 | Jesus Alberto Mejia Villarreal | @Jesss0191 | Tabla de datos (Excel) Repositorio (Github) |
| 2 | Laura Sofía Salcedo Bedoya | @Lau777479 | Análisis gráfico (Colab/Conda) |
| 3 | Valentina Cardenal Moyano | @merlin0612 | Informe en LaTeX |
| 4 | Jean Paul Rivera Romero | @JeanpRivera | Presentación (Power BI) |
| 5 | Laura María Espinosa Bernal | @Laura-EB153 | Informe en LaTeX |

## 🧑‍🚀 Objetivos

**General**

- Analizar y comparar las propiedades físico-químicas de halogenuros de alquilo y acilo mediante herramientas de análisis y visualización de datos, relacionando las tendencias observadas con la estructura de cada sustancia.

**Específicos**

- Construir una tabla de datos completa y organizada con las propiedades químicas, indicando la fuente de cada dato.
- Desarrollar un análisis gráfico en Conda o Google Colab que muestre tendencias y probabilidad, y relacione las propiedades entre sí.
- Redactar un informe en LaTeX con los resultados y su argumentación.
- Diseñar un dashboard en Power BI integrado al modelo de datos y preparar la exposición.
- Trabajar de forma colaborativa en GitHub, con seguimiento de todos los integrantes y tareas organizadas en un Project.

## 👨‍🔬 Metodología

Recolección de datos

La información se obtuvo de la plataforma CAS-SciFinder para diez sustancias halogenadas: clorometano, diclorometano, cloroformo, tetracloruro de carbono, cloruro de formilo, bromoetano, fluoroetano, fluoruro de acetilo, bromuro de acetilo y bromociclohexano. Para cada una se consultaron el peso molecular, el punto de fusión, el punto de ebullición, la densidad, el pKa, el momento dipolar, la solubilidad en agua y la presión de vapor. Además, se registraron diez reacciones, con las mismas propiedades para el producto principal, y diez obtenciones, con las mismas propiedades para el reactante. De cada reacción u obtención se anotaron el número de reacción CAS, los catalizadores, reactivos y solventes, la temperatura, el medio, el nombre y el tipo de reacción y, en el caso de las reacciones, los productos. Todo se organizó en un libro de Excel con tres hojas: Compuestos, Reacciones y Obtenciones.

Organización y revisión de los datos

Los datos se depuraron para poder leerlos directamente en Python y en Power BI. Las celdas sin información se dejaron vacías en lugar de usar texto como “No aplica”, los valores se guardaron como números con punto decimal y se unificó la notación científica. Cuando una propiedad aparecía como rango se tomó el valor menor, lo mismo que cuando había dos valores de pKa, y cuando la fuente daba una desigualdad se usó el número del límite. Los valores con errores evidentes de formato, como decimales perdidos o datos que Excel había convertido en fechas, se revisaron y corrigieron, y también se corrigieron nombres con errores de escritura. Se conservó una única versión final de la tabla, y las versiones intermedias quedaron en el repositorio como registro del proceso.

Análisis gráfico

El análisis se desarrolló en Google Colab con Python. El notebook carga la tabla de datos, prepara las columnas numéricas y genera las gráficas, cada una acompañada de una celda de texto en formato Markdown que explica el proceso realizado y el resultado. Se elaboraron comparaciones de cada propiedad entre los diez compuestos, un mapa de calor de las propiedades fisicoquímicas, distribuciones de variables como la solubilidad, gráficos de la frecuencia de los tipos de reacción y del número de reacciones y obtenciones por compuesto, y gráficos de áreas apiladas del peso molecular de los productos por reacción. Estas visualizaciones permiten identificar tendencias entre propiedades y relacionarlas con la estructura de cada sustancia.

Informe en LaTeX

El informe se redactó en LaTeX con formato de artículo de investigación, para obtener un documento con estructura, espacio y ubicación de los contenidos consistentes. Incluye introducción, metodología, resultados y conclusiones, e integra las tablas y las figuras generadas en el análisis gráfico. La redacción se repartió entre varios integrantes del grupo, los avances de cada versión se guardaron en el repositorio y el documento final se compiló a PDF.

Visualización en Power BI

La tabla de datos se importó a Power BI y se construyó un modelo que relaciona la hoja de compuestos con las de reacciones y obtenciones a través del nombre de cada compuesto, de modo que los filtros se apliquen de forma coherente en todas las páginas. Sobre este modelo se diseñó una presentación interactiva, con segmentaciones y gráficos enlazados, que permite explorar las propiedades, los tipos de reacción y las condiciones de cada una por compuesto, y que sirve de apoyo en la exposición.

Gestión del trabajo en GitHub

GitHub se usó como el espacio central de trabajo del grupo para desarrollar y organizar el proyecto de forma colaborativa. En el repositorio se guardó cada entregable (la tabla de datos en Excel, las gráficas y el notebook de Colab, el informe en LaTeX y el archivo de Power BI), junto con la rúbrica y el enunciado en una carpeta de documentos. Cada carpeta se dividió en una parte de proceso y otra final, de modo que las versiones sucesivas de la tabla de datos (de la V1 a la V12) y los avances del informe y de las gráficas quedaron registrados y se pueden consultar o recuperar. El historial de casi 70 commits permite ver qué aportó cada uno de los cinco integrantes y cuándo, y evita que el trabajo se pierda o se sobrescriba al editar entre varias personas. El README documenta la descripción del proyecto, los objetivos, la metodología, el reparto de responsabilidades y las fechas, y un GitHub Project sirvió para organizar y asignar las tareas.


## 📂 Estructura del repositorio

```
.
├── README.md
├── Datos/          # Carpeta compuesta de dos tipos de bases de datos en formato `.xlsx`, con información extraída de **CAS-SciFinder**:
    ├── Datos/Proceso/          # Contiene borradores de las tablas de datos, actualizados a medida que se completaba la información reflejando el progreso del proyecto
    ├── Datos/Final/          # Contiene el archivo final con las 100 reacciones y 100 obtenciones junto a las propiedades de los 10 compuestos a analizar
├── Notebooks/      # Análisis gráfico (.ipynb) – Colab
    ├── Notebooks/Proceso/          # Contiene avances de las gráficas realizadas en colab, editadas mediante correcciones
    ├── Notebooks/Final/          # Contiene las gráficas finales hechas en Google colab junto a la explicación de cada proceso 
├── Informe/        # Informe en LaTeX (.tex, .bib, figuras y PDF compilado)
    ├── Informe/Proceso/          # Contiene avances del informe LaTeX
    ├── Informe/Final/          # Contiene el informe LaTeX completo
├── Power BI/        # Archivo .pbix y capturas de los dashboards
    ├── Power BI/Modificación/          # Contiene los archivos necesarios para modificar la presentación de power bi
    ├── Power BI/Final/          # Contiene el archivo final .pbix con la presentación del proyecto
└── Docs/           # Rúbrica, enunciado y notas del grupo
```


## 📅 Fechas

- **Entrega:** 16 de noviembre, hasta las 18:00 (carpeta comprimida organizada)
- **Exposiciones:** 19, 23 y 26 de noviembre (orden por número de proyecto)
- **Duración:** 25 min (10 de exposición, 12 de preguntas, 3 de revisión previa)

## 🛠️ Tareas del Project (tablero)

- [✅] Crear repositorio, agregar a los 5 integrantes y crear el Project
- [✅ ] Definir sustancias y propiedades a incluir en la tabla
- [✅ ] Construir y revisar la tabla de datos
- [✅ ] Cargar datos y limpiar en el notebook
- [✅ ] Gráficas: tendencias y relación entre propiedades
- [✅ ] Documentar las líneas de código del notebook
- [✅ ] Estructura del informe en LaTeX
- [✅ ] Redactar secciones del informe 
- [✅ ] Compilar PDF y revisar errores
- [✅ ] Modelo y dashboards en Power BI
- [✅ ] Preparar exposición (10 min) y ensayar preguntas
- [✅ ] Verificar clonado/descarga del repo desde cero
- [✅ ] Comprimir carpeta y entregar antes del 16/11, 18:00
