# Test_Gradle
  Creación automática con gradle
  Primero verificamos que tenemos instalado el jdk de java:
  <pre><code>java -version </code></pre>
  `![texto cualquiera por si no carga la imagen](url completa de la imagen)`
  También verificamos que el gradle esté en el path:
  <pre><code>gradle -version </code></pre>
  `![texto cualquiera por si no carga la imagen](url completa de la imagen)`
  Una vez verificado , Vamos ejecutar algunas tareas listadas con la sentencia gradle -q tasks. Como vemos, tomaremos la sentencia gradle help –task,  la cual nos mostrará la ayuda de una tarea específica , le pediremos a Gradle que  nos muestre información de la tarea ‘init’..
  <pre><code>gradle -q help --task init </code></pre>
  `![texto cualquiera por si no carga la imagen](url completa de la imagen)`
  Ahora que ya sabemos que la tarea ‘init’ crea la estructura inicial de directorio en nuestro proyecto y  además nos brinda las opciones que tenemos para ejecutar la tarea init, procederemos desde una terminal a ejecutar:
  <pre><code>gradle init --project-name myproyect --type basic </code></pre>
  `![texto cualquiera por si no carga la imagen](url completa de la imagen)`
  
  
