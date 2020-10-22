# Test_Gradle
  ## Creación automática con gradle<br/>
  Primero verificamos que tenemos instalado el jdk de java:
  <pre><code>java -version </code></pre>
  ![texto cualquiera por si no carga la imagen](https://github.com/JoseCcari/Test_Gradle/blob/main/JAVA-VERSION.PNG)
  También verificamos que el gradle esté en el path:
  <pre><code>gradle -version </code></pre>
  ![texto cualquiera por si no carga la imagen](https://github.com/JoseCcari/Test_Gradle/blob/main/GRADLE.PNG)
  Una vez verificado , Vamos ejecutar algunas tareas listadas con la sentencia gradle -q tasks. Como vemos, tomaremos la sentencia gradle help –task,  la cual nos mostrará la ayuda de una tarea específica , le pediremos a Gradle que  nos muestre información de la tarea ‘init’..
  <pre><code>gradle -q help --task init </code></pre>
  ![texto cualquiera por si no carga la imagen](https://github.com/JoseCcari/Test_Gradle/blob/main/java-help.PNG)
  Ahora que ya sabemos que la tarea ‘init’ crea la estructura inicial de directorio en nuestro proyecto y  además nos brinda las opciones que tenemos para ejecutar la tarea init, procederemos desde una terminal a ejecutar:
  <pre><code>gradle init --project-name myproyect --type basic </code></pre>
  ![texto cualquiera por si no carga la imagen](https://github.com/JoseCcari/Test_Gradle/blob/main/ini_gradle.PNG)
  
  ## Una visión general de lo que nos construyó la tarea init con el type basic.
Nos creó dos archivos en la raíz del proyecto con los nombres build.gradle y settings.gradle. Estos archivos son utilizados por Gradle para la configuración de construcción del proyecto.

### build.gradle:
Archivo de texto plano que mediante del lenguaje específico de dominio(DSL). En este archivo especificamos los tipos de empaquetados y el producto que requerimos al compilar (jar, war, etc). También especificamos los repositorios y dependencias que se necesitarán al momento de compilar. Además, puedes definir propiedades del archivo manifiesto.

### settings.gradle: 
Archivo de texto plano que indica a gradle los módulos que deberá incluir al momento de compilar el proyecto.

También nos creó un directorio Gradle el cual almacena el wrapper. Wrapper es un script que invoca una versión declarada de Gradle, el cual lo descarga si es necesario. Los archivos que componen wrapper son:

### gradle-wrapper.jar:
El archivo Wrapper JAR que contiene el código para descargar la distribución Gradle.

### gradle-wrapper.properties: 
Un archivo de propiedades responsable de configurar el comportamiento del tiempo de ejecución Wrapper, p. La versión Gradle compatible con esta versión. Tenga en cuenta que las configuraciones más genéricas, como configurar el Wrapper para usar un proxy, deben ir a un archivo diferente.

 ### gradlew: 
 script para sistemas basado en UNIX, almacenado en el directorio raíz del proyecto para ejecutar gradle-wrapper.

### gradlew.bat: 
script para sistemas Windows, almacenado en el directorio raiz del proyecto para ejecutar gradle-wrapper.

 Los scripts gradlew y gradlew.bat son los que recomienda gradle ejecutar con las tareas una vez que se inicializó el proyecto.
  
  
