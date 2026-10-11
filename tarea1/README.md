**UEA y clave:** [Administracion de proyectos de software] - [1151055]
**Trimestre:** [26-O]
**Licenciatura:** Ingeniería en Computación
**Nombre:** Ricardo Daniel García Roldán
**Matrícula:** [2222003341]

--
1. ¿Qué es un proyecto de software? Proyecto frente a operación continua; proyecto, producto y proceso; alcance, tiempo, costo y calidad.
Es un esfuerzo temporal que se lleva a cabo para crear un producto, servicio o resultado único. Se diferencia de una operación continua en que esta última es un trabajo repetitivo y permanente que sostiene el negocio diario, mientras que el proyecto tiene un inicio y un fin definidos.
Alcance: Todo el trabajo que debe realizarse para entregar el producto.
Tiempo: El cronograma y los plazos de entrega.
Costo: El presupuesto asignado (horas hombre, infraestructura).
Calidad: El cumplimiento de los requisitos explícitos e implícitos del software

--
2. ¿Cómo se administra? Qué son la Guía del PMBOK y Scrum, y en qué se distinguen los modelos predictivo, iterativo y ágil. Cuál elegiría para un proyecto como el del curso.
La administración de proyectos consiste en aplicar conocimientos, habilidades, herramientas y técnicas para cumplir con los requisitos del proyecto y generar valor.
La Guía del PMBOK (Project Management Body of Knowledge): Es un estándar global editado por el Project Management Institute (PMI). No es una metodología rígida, sino un compendio de buenas prácticas y fundamentos. 
Scrum: Es un marco de trabajo (framework) específico y ágil diseñado para el desarrollo y entrega incremental de productos complejos. Se fundamenta en equipos autoorganizados y roles fijos (Product Owner, Scrum Master y Equipo) que operan mediante ciclos cortos de tiempo fijos (llamados Sprints).
Los modelos de gestión se distinguen por cómo manejan el cambio y la entrega:
Predictivo (Cascada): El alcance, tiempo y costo se determinan en las fases iniciales. Los cambios son difíciles y costosos.
Iterativo: El alcance se determina temprano, pero el tiempo y costo se modifican a medida que el equipo comprende mejor el producto. Se entrega en versiones sucesivas.
Ágil: Orientado al cambio continuo. Es iterativo e incremental; el alcance se define y redefine antes del inicio de cada iteración corta.
Escogería scrum para poder moldear los requisitos del proyecto a medida que aprendo nuevas tecnologías y para hacer pequeñas entregas de código funcional

--
3. ¿Con qué herramientas? Para qué sirven el control de versiones, los tableros de trabajo, los contenedores y la integración continua. Y las del curso: Docker frente a una máquina virtual, Dockerfile frente a compose.yaml, el volumen, y los comandos up -d, exec, stop, down, ps y logs.
• Control de versiones: Sirve para registrar los cambios realizados en el código fuente a lo largo del tiempo. Permite que múltiples desarrolladores trabajen simultáneamente sin sobrescribir su trabajo, mantiene un historial completo y facilita la recuperación de versiones anteriores si ocurre un error.
• Tableros de trabajo: Sirven para gestionar y visualizar el flujo de trabajo de un proyecto. Ayudan a organizar tareas (por hacer, en proceso, completadas), asignar responsabilidades, estimar tiempos y mantener la transparencia dentro del equipo.
• Contenedores: Sirven para empaquetar una aplicación junto con todas sus dependencias, bibliotecas y configuración en una sola unidad ligera. Esto garantiza que la aplicación se ejecute exactamente igual en la computadora de un desarrollador, en un servidor de pruebas o en la nube.
• Integración Continua: Sirve para automatizar la fusión de los cambios de código de distintos desarrolladores en un repositorio central. Cada vez que se sube código, se ejecutan pruebas automáticas para detectar errores de forma temprana y asegurar que el proyecto siga siendo estable.
Docker frente a una Máquina Virtual (VM): Una VM virtualiza el hardware completo e incluye un sistema operativo huésped completo (pesado). Docker virtualiza a nivel del sistema operativo; los contenedores comparten el kernel del host, haciéndolos ligeros y rápidos de iniciar.
Dockerfile frente a compose.yaml: El `Dockerfile` es la receta (instrucciones) para construir una única imagen de contenedor. El `compose.yaml` es un archivo de orquestación que define cómo ejecutar y comunicar múltiples contenedores juntos (bases de datos, backend, frontend).
Volumen: Es un mecanismo para persistir datos generados por el contenedor, evitando que se borren cuando el contenedor se destruye.
Comandos:
  up -d: Levanta los contenedores en segundo plano (detached).
  exec: Ejecuta un comando dentro de un contenedor que ya está corriendo.
  stop: Detiene un contenedor en ejecución sin borrarlo.
  down: Detiene y elimina los contenedores, redes y volúmenes creados por compose.
  ps: Muestra la lista de contenedores en ejecución.
  logs: Muestra la salida de consola (registros) de un contenedor.

--
4. ¿Bajo qué licencia se distribuye el software? Todo programa tiene una licencia que dice qué puede hacer con él quien lo recibe —usarlo, modificarlo, redistribuirlo, venderlo— y con qué obligaciones.
Usted eligió una al crear su repositorio. Investigue:
a) Los dos grandes tipos. Qué es una licencia permisiva (MIT, BSD, Apache 2.0) y qué es una copyleft
(GPL, LGPL, AGPL). Una tabla con lo que permite y lo que exige cada una.
Permisivas (MIT, BSD, Apache 2.0): Permiten hacer prácticamente cualquier cosa con el código, incluyendo integrarlo en software propietario de código cerrado, con mínimas restricciones (casi siempre solo exigir que se mantenga el aviso de derechos de autor).
Copyleft (GPL, LGPL, AGPL): Garantizan que el software y todas sus versiones derivadas permanezcan libres. Si modificas y distribuyes el código, estás obligado a liberar tus modificaciones bajo la misma licencia.
| Característica | Permisiva | Copyleft |
| :--- | :--- | :--- |
| **Uso comercial** | Permitido | Permitido |
| **Modificación y distribución** | Permitido | Permitido |
| **Integración en software cerrado**| Permitido | Prohibido (exige abrir el código derivado) |
| **Exigencia principal** | Mantener el aviso de autoría | Distribuir obras derivadas bajo la misma licencia |

b) Su elección. Por qué su repositorio usa MIT, qué ventajas tiene y qué cambiaría si hubiera elegido GPL.
Se seleccionó por su simplicidad y la máxima libertad que otorga a la comunidad. Permite que cualquier desarrollador o empresa use, modifique, distribuya e incluso venda el software sin temor a restricciones legales complejas o auditorías de licencias infectadas.
Si se hubiese optado por la licencia GNU GPL, el proyecto ganaría protección comunitaria pero perdería flexibilidad comercial. Cualquier entidad que tomara este código para modificarlo y distribuirlo dentro de su propia aplicación estaría obligada legalmente a liberar todo el código fuente de su aplicación bajo GPL.

c) Un caso real, a elegir, en que la decisión de la empresa dueña de un proyecto llevó a sus usuarios
a crear o adoptar una alternativa:
– MySQL, que pasó a manos de Oracle, y MariaDB.
– El JDK de Oracle, que empezó a cobrarse para uso comercial, y OpenJDK o Amazon Corretto.
– CentOS, que Red Hat sustituyó por CentOS Stream, y AlmaLinux o Rocky Linux.
Cuente qué pasó y cuándo, qué licencia tenía el proyecto, y la clave: por qué esa licencia permitió
que la alternativa existiera sin pedirle permiso a nadie.
Java Development Kit (JDK) de Oracle era gratuito para la mayoría de los casos de uso. Sin embargo, a partir de abril de 2019 (coincidiendo con las actualizaciones de Java SE 8 y el lanzamiento de Java 11), Oracle cambió drásticamente sus términos de licenciamiento comercial. Introdujo la licencia Oracle Technology Network (OTN), que permitía el uso gratuito para desarrollo y pruebas personales, pero exigía el pago de tarifas de suscripción comercial para su ejecución en entornos de producción empresarial.
Ante el temor de auditorías y costes inesperados, la comunidad y los grandes proveedores de la nube buscaron alternativas estables y gratuitas a largo plazo. Como respuesta directa, empresas como Amazon lanzaron Amazon Corretto a finales de 2018 y principios de 2019.
¿Qué licencia tenía el proyecto?
El lenguaje Java y las especificaciones base se desarrollan bajo el proyecto de código abierto OpenJDK, el cual está licenciado bajo la Licencia Pública General de GNU, versión 2, con la Excepción de Classpath (GPLv2 + CPE).

Ejercicio 3. De PostgreSQL 17 a 18

1. Diferencias entre los dos contenedores

| Qué decía (PostgreSQL 17) | Qué dice (PostgreSQL 18) | Por qué cambió |
| :--- | :--- | :--- |
| **Archivo:** `docker-compose.yml` | **Archivo:** `compose.yaml` | `compose.yaml` es el nombre estándar y recomendado por la Compose Specification moderna (Compose V2). |
| **Construcción:** `image: postgres:17` | **Construcción:** `build: .` e `image: postgres-1151055:26o` | En la v17 se bajaba la imagen oficial directa. En la v18 se construye una imagen personalizada local usando el Dockerfile (para instalar nano, less, etc.) y se le asigna un nombre propio. |
| **Volúmenes:** `./data:/var/lib/postgresql/data` | **Volúmenes:** `datos_db:/var/lib/postgresql` | Hubo dos cambios: 1) Postgres 18 cambió su ruta interna de datos. 2) Se pasó de usar un "bind mount" (carpeta local `./data`) a un volumen administrado por Docker (`datos_db`). |
| **Variables:** Valores fijos (ej. `POSTGRES_DB: postgres`) | **Variables:** Valores por defecto (ej. `${POSTGRES_DB:-proyecto}`) | La sintaxis `:-` permite que el contenedor levante con un valor por defecto si no existe un archivo `.env`, haciéndolo más flexible. |
| **Salud:** No tenía configuración de salud. | **Salud:** Bloque `healthcheck` con `pg_isready`. | Sirve para que Docker sepa exactamente cuándo la base de datos está lista para recibir conexiones por la red. |
| **Servicios:** Solo existía el servicio `postgres`. | **Servicios:** Se añadió el servicio `adminer`. | Se agregó una interfaz gráfica web ligera que depende de que la base de datos esté "healthy" para poder iniciar. |

2. ¿Se usaba el Dockerfile viejo?
No, no se usaba.** Aunque el archivo `Dockerfile` existía físicamente en la carpeta de la versión 17, si revisamos el archivo `docker-compose.yml` viejo, el servicio de base de datos solo tenía la instrucción `image: postgres:17`. Al no incluir la instrucción `build: .` (que es la que le ordena a Compose leer el Dockerfile), Docker ignoró ese archivo por completo y simplemente descargó la imagen oficial ya hecha desde Docker Hub.

3. Versionado semántico y el salto a la 18
El versionado semántico es una convención para numerar el software usando tres números: `MAYOR.MENOR.PARCHE`. 
Pasar de la versión 17 a la 18 representa un **cambio MAYOR**. En el versionado semántico, cuando el primer número cambia, significa que se introdujeron modificaciones drásticas que rompen la compatibilidad con versiones anteriores (*breaking changes*). En el caso de PostgreSQL, un cambio mayor implica que la estructura interna en la que se guardan los archivos de la base de datos cambia; por eso, el contenedor de la versión 18 no puede leer los datos (el volumen) que había guardado la versión 17 sin hacer antes una migración manual.

Ejercicio 4

1. Tabla comparativa: PostgreSQL + Adminer frente a MySQL + phpMyAdmin

| Característica | PostgreSQL + Adminer | MySQL + phpMyAdmin |
| :--- | :--- | :--- |
| **Motor de Base de Datos** | **PostgreSQL:** Sistema objeto-relacional muy estricto con el estándar SQL. Ideal para transacciones complejas, integridad de datos rígida y analítica. | **MySQL:** Sistema relacional tradicionalmente enfocado en la velocidad de lectura. Es la base histórica de una gran parte de la web (stack LAMP). |
| **Interfaz Web** | **Adminer:** Herramienta ultraligera (un solo archivo PHP). Su interfaz es minimalista y permite conectarse a múltiples motores de bases de datos, no solo PostgreSQL. | **phpMyAdmin:** Herramienta pesada y robusta, exclusiva para gestionar MySQL y MariaDB. Ofrece una interfaz gráfica con múltiples asistentes y opciones visuales. |

2. Versiones LTS, Innovation y el uso de etiquetas específicas
Versión LTS (Long Term Support): Son versiones enfocadas en la estabilidad a largo plazo. No reciben nuevas funciones experimentales, pero garantizan parches de seguridad y correcciones de errores durante años. Son el estándar para entornos de producción.
Versión Innovation: Son versiones que se liberan con frecuencia para introducir las características y tecnologías más recientes. Su ciclo de vida oficial es corto, obligando a los equipos a actualizar constantemente.

¿Por qué se usa `mysql:9.7.2` y no `mysql:latest`?
Usar la etiqueta `latest` es una mala práctica en la administración de proyectos de software porque rompe la reproducibilidad. La etiqueta `latest` es un puntero móvil: hoy puede descargar la versión 8, pero si mañana sale la versión 9 (con cambios mayores que rompen la compatibilidad), el sistema la descargará automáticamente y la aplicación dejará de funcionar. 

Al fijar la versión exacta (`9.7.2`), se garantiza que el entorno de desarrollo sea predecible e idéntico para cualquier persona del equipo que levante el contenedor, sin importar en qué año lo haga.

Para la elaboración de este documento, se utilizó inteligencia artificial (Gemini) como asistente de apoyo para el formateo de las tablas en Markdown y la revisión de estilo en la redacción de los textos.

Bibliografia:
Chacon, S., & Straub, B. (2014). *Pro Git* (2a ed.). Apress.
Free Software Foundation. (2021). *What is free software?*. The GNU Operating System. https://www.gnu.org/philosophy/free-sw.html
Open Source Initiative. (2023). *The MIT License*. https://opensource.org/licenses/MIT
Project Management Institute. (2021). *Guía de los Fundamentos para la Dirección de Proyectos (Guía del PMBOK)* (7a ed.). Project Management Institute.
Schwaber, K., & Sutherland, J. (2020). *La Guía de Scrum*. Scrum.org. https://scrumguides.org/
Sommerville, I. (2015). *Software Engineering* (10a ed.). Pearson.
Turnbull, J. (2014). *The Docker Book: Containerization is the new virtualization*.
