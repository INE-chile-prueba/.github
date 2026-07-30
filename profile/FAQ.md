# Preguntas Frecuentes (FAQ)

Bienvenido al centro de preguntas y respuestas frecuentes de los repositorios de la Subdirección Técnica del Instituto Nacional de Estadísticas de Chile (INE).


## 1. Sobre el Repositorio y los Datos

<details>
  <summary><b>¿Qué contiene este repositorio?</b></summary>
  <br>
  Este repositorio reúne código fuente, scripts y funciones desarrollados o utilizados por la Subdirección Técnica del Instituto Nacional de Estadísticas de Chile (INE), asociados a la construcción y reproducción de productos estadísticos publicados por la institución.<br><br>
  Su contenido está destinado a facilitar la reproducibilidad y transparencia de los resultados estadísticos, poniendo a disposición los códigos de programación utilizados para la elaboración de cuadros estadísticos publicados en <a href="https://ine.gob.cl">ine.gob.cl</a>, correspondientes a algunas de las operaciones estadísticas del INE que cuentan con bases de datos públicas disponibles.<br><br>
  Cada repositorio indica en su descripción la operación estadística y el producto estadístico asociado, los resultados que permite reproducir.
</details>

<details>
  <summary><b>¿A quién está dirigido?</b></summary>
  <br>
  Está dirigido a personas interesadas en las estadísticas oficiales y su procesamiento, como investigadores, periodistas, académicos, estudiantes, analistas de datos y desarrolladores. Para ejecutar algunos proyectos se requieren conocimientos básicos de programación en el lenguaje señalado en el repositorio.
</details>

<details>
  <summary><b>¿El código forma parte de una publicación estadística oficial?</b></summary>
  <br>
  El código complementa la documentación disponible y no reemplaza los productos oficiales publicados por el INE. Si tras la ejecución de estos códigos existiese alguna diferencia respecto de la información oficial publicada en <a href="https://ine.gob.cl">ine.gob.cl</a>, prevalecen las cifras, definiciones, notas técnicas y documentos difundidos en dicho sitio web.<br><br>
  Los códigos contenidos en este repositorio utilizan exclusivamente las bases de datos públicas del INE, las que han pasado por un estricto proceso de anonimización (para más detalles véase la <a href="https://ine.gob.cl/docs/default-source/buenas-practicas/directrices-metodologicas/guias-y-orientaciones-metodologicas/documentos/guía-control-divulgación-estadística-microdatos.pdf">Guía de control de divulgación estadística de microdatos</a>).
</details>

<details>
  <summary><b>¿Puedo considerar como datos oficiales aquellos resultados que obtengo de la ejecución de estos códigos?</b></summary>
  <br>
  No, sólo la información que publica el INE en su sitio web tiene el carácter de oficial. El objetivo de este repositorio es facilitar el manejo de las bases de datos públicas. Los resultados de la aplicación y/o modificación de estos scripts por parte de los usuarios son de su propia responsabilidad y podrán ser citados como “Elaboración propia en base a datos del INE”.
</details>

<details>
  <summary><b>¿Todos los repositorios contienen datos?</b></summary>
  <br>
  No. Los repositorios sólo incluyen código de programación, algunos pueden contener plantillas de Excel o instrucciones para obtener los datos desde una fuente oficial. El README de cada Operación Estadística indica los archivos fuentes necesarios (bases de datos públicas) y señala desde dónde se obtienen.
</details>

<details>
  <summary><b>¿Los datos incluidos son oficiales y están actualizados?</b></summary>
  <br>
  Cada repositorio indica la fuente, fecha de extracción, periodo de referencia y estado de los datos utilizados. Antes de publicar o citar resultados, se recomienda comprobar si existen versiones más recientes o rectificaciones en el sitio oficial del INE.
</details>

<details>
  <summary><b>¿El repositorio contiene datos personales o información confidencial?</b></summary>
  <br>
  No. Los repositorios sólo incluyen código de programación, algunos pueden contener plantillas de Excel o instrucciones para obtener los datos desde una fuente oficial. Los scripts hacen lectura de microdatos públicos de <a href="https://ine.gob.cl">ine.gob.cl</a> y estos corresponden a archivos anonimizados según las normas de anonimización publicadas en la <a href="https://ine.gob.cl/docs/default-source/buenas-practicas/directrices-metodologicas/guias-y-orientaciones-metodologicas/documentos/guía-control-divulgación-estadística-microdatos.pdf">Guía de control de divulgación estadística de microdatos</a>.
</details>

---

## 2. Uso, Ejecución y Aspectos Técnicos

<details>
  <summary><b>¿Cómo se descarga el código?</b></summary>
  <br>
  Se puede utilizar cualquiera de estas alternativas:
  <ol>
    <li>Seleccionar <b>Code</b> y luego <b>Download ZIP</b>.</li>
    <li>Clonar el repositorio mediante Git: <br><code>git clone https://github.com</code></li>
  </ol>
  La descarga en ZIP es suficiente para consultar o ejecutar el contenido. La clonación con Git facilita recibir actualizaciones y consultar el historial de cambios.
</details>

<details>
  <summary><b>¿Qué programa necesito para ejecutar el código?</b></summary>
  <br>
  Depende del lenguaje utilizado. El README de cada repositorio indica:
  <ul>
    <li>Lenguaje y versión.</li>
    <li>Paquetes o bibliotecas requeridos.</li>
    <li>Sistema operativo probado.</li>
    <li>Programas adicionales necesarios.</li>
    <li>Instrucciones de instalación.</li>
  </ul>
  En proyectos desarrollados en R o Python, se recomienda utilizar las versiones y dependencias declaradas en archivos como <code>renv.lock</code>, <code>requirements.txt</code>, <code>environment.yml</code>, <code>pyproject.toml</code> u otros equivalentes.
</details>

<details>
  <summary><b>¿En qué orden deben ejecutarse los archivos?</b></summary>
  <br>
  El orden debe estar descrito en el README de cada repositorio particular. No debe suponerse que el orden alfabético de los archivos corresponde al orden de ejecución.
</details>

<details>
  <summary><b>¿Por qué el código no encuentra un archivo?</b></summary>
  <br>
  Las causas más habituales son:
  <ul>
    <li>El archivo no fue descargado.</li>
    <li>Fue guardado en una carpeta distinta.</li>
    <li>Cambió su nombre.</li>
    <li>La ruta está escrita para otro sistema operativo.</li>
    <li>El nombre contiene diferencias de mayúsculas, espacios o caracteres especiales.</li>
    <li>El archivo debe obtenerse desde una fuente externa.</li>
  </ul>
  Se recomienda revisar la sección de datos de entrada y la estructura de carpetas del proyecto antes de modificar el código.
</details>

<details>
  <summary><b>¿Por qué aparece un error al instalar o cargar un paquete?</b></summary>
  <br>
  En general los repositorios usan <code>.renv</code>, lo que garantiza que su ejecución se realizará con las librerías y versiones que fueron utilizadas al momento de la construcción de los scripts.<br><br>
  Puede deberse a una versión incompatible del lenguaje, una dependencia faltante, restricciones de conexión o cambios posteriores en el paquete. La primera medida es reproducir las versiones indicadas en el repositorio. Si el problema persiste, puede informarse mediante una solicitud de soporte institucional.
</details>

<details>
  <summary><b>¿Puedo ejecutar solamente una parte del proyecto?</b></summary>
  <br>
  Depende de las relaciones entre los scripts. Un archivo puede requerir resultados generados por etapas anteriores. El README debería distinguir los componentes independientes de aquellos que forman una secuencia obligatoria.
</details>

<details>
  <summary><b>¿Cuánto tarda la ejecución?</b></summary>
  <br>
  El tiempo depende del volumen de datos, las características del equipo y las etapas ejecutadas. Cuando una operación sea prolongada o requiera mucha memoria, es posible que la información de estimación de tiempo esté incluida en el README del repositorio.
</details>

<details>
  <summary><b>¿Al ejecutar el código obtendré exactamente las cifras publicadas por el INE?</b></summary>
  <br>
  Se deberían obtener los resultados indicados cuando se utilicen los mismos datos de entrada, versiones de software, parámetros y secuencia de ejecución. Pueden existir diferencias cuando:
  <ul>
    <li>Los datos fueron actualizados o rectificados.</li>
    <li>Cambiaron las dependencias.</li>
    <li>El sistema aplica una precisión numérica diferente.</li>
    <li>Alguna etapa requiere información no incluida en el repositorio.</li>
  </ul>
  El README identifica la publicación y la versión de los datos que el código permite reproducir. Los códigos contenidos en este repositorio utilizan exclusivamente las bases de datos públicas del INE (anonimizadas), por lo que los resultados obtenidos pueden variar respecto de los resultados obtenidos durante la etapa de procesamiento interno, lo que será advertido en el README del respectivo repositorio.
</details>

<details>
  <summary><b>¿Qué resultados debería generar el proyecto?</b></summary>
  <br>
  Cada repositorio enumera los archivos de salida esperados, su ubicación y su relación con las tablas, gráficos, indicadores o documentos publicados.
</details>

<details>
  <summary><b>¿Por qué mis resultados difieren de los publicados?</b></summary>
  <br>
  Primero se deben comprobar:
  <ul>
    <li>Versión de los datos.</li>
    <li>Periodo de referencia.</li>
    <li>Filtros y parámetros.</li>
    <li>Versiones de R, Python o del lenguaje utilizado.</li>
    <li>Dependencias instaladas.</li>
    <li>Orden de ejecución.</li>
    <li>Tratamiento de valores perdidos.</li>
