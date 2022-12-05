# Sistemas Operativos
## ¿Qué hace un sistema operativo?
Un sistema operativo es una interfaz o programa que permite al usuario trabajar con los componentes de un dispositivo electrónico.
Algunos de los servicios que ofrece un sistema operativo son:
- Ejecución de programas
- Operaciones de Entrada/Salida
- Manipulación de archivos y directorios
- Comunicación entre procesos
- Comunicación con equipos remotos
- Administración de la protección y seguridad
- Leer el estado del sistema

## ¿Qué es el OpenSource?
También denominado código abierto, se refiere cuando un software permite al usuario poder utilizar el código fuente para realizar cambios y modificaciones a preferencia del usuario.
Las principales características de un código open source son:
- Habilidad de ser copiado, modificado y editado por terceros sin ningún costo.
- Acceso completo al código fuente.
- La licencia del software debe permitir cambios y modificaciones.
- Debe ser disponible a todos los tipos de usuarios.
- La licencia debe poderse compartir por cualquier medio.

Ejemplos de programas Open Source:
- GNU Compiler Collection (Conjunto de herramientas de compilación para C,C++)
- GNOME (Entorno de escritorio del sistema operativo Linux)
- KDE (Entorno de escritorio del sistema operativo Linux)
- Moodle (Sistema de aprendizaje virtual)
- Firefox (Navegador web basado en Mozilla)

## Comandos básicos de la terminal UNIX
- cd (Cambiar de carpeta o directorio)
- cd .. (Retroceder una carpeta o directorio)
- pwd (Nombrar el directorio en el que se encuentra actualemente el usuario)
- ls (Mostrar los archivos en esa carpeta o directorio)
- ls -la (Mostrar los archivos, incluyendo los ocultos, en esa carpeta o directorio con información extra)
- mkdir newFolder (Crear una carpeta dentro del directorio actual)
- touch fileName (Crear un archivo dentro de la carpeta o directorio actual)
- rm fileName (Eliminar un archivo con el nombre indicado)
- vim fileName (Abrir un archivo con el editor vim)
- history (Muostrar el historial de comandos)
- git init (Iniciar un repositorio de git)
- git add . (Agregar todos los cambios en la máquina local)
- git commit -m "mensaje" (Guardar un cambio hecho en el repositorio)
- git push (Subir cambios al cliente remoto del usuario como github)

## Dispositos de entrada/salida
### Dispositivos de entrada
Los dispositivos de entrada son aquellos equipos encargados de introducir datos en la memoria central de la computadora para su tratamiento. A través de ellos se transforma la información de entrada en señales eléctricas.
Ejemplos de dispositos de entrada:
- Teclado
- Mouse
- Cámara de video o webcam
- Lectora de código de barras

### Dispositivos de salida
Los dispositivos de salida son los equipos que presentan la información al usuario de forma comprensible, ya sea a través de imágenes, texto, sonido o táctil. Estos realizan la función de extraer datos de la memoria central hacia el exterior.
Ejemplos de dispositivos de salida:
- Pantalla o monitor
- Bocinas
- Impresora
- Robot

### Dispositivos mixtos
Los dispositivos mixtos permiten la introducción y extracción de datos en la memoria central.
Ejemplos de dispositivos mixtos:
- Pantalla o monitor táctil
- Impresora multifunción con funciones de imprimir, escanear y fotocopiar

## Procesos
Un proceso es el nombre que se le da a la ejecución de un programa individual, representado por una serie de instrucciones que el procesador debe ejecutar.
La UCP (Unidad Central de Procesos) es quien se encarga de ordenar la ejecución de los procesos según diversos factores.
Un proceso puede tener subprocesos con sus propias series de instrucciones y consumo de recursos propios. Los subprocesos reciben el nombre de hebras o hilos.
### Características de un proceso
- Identificador: Número entero que se le asigna a un proceso para distinguirlo del resto.
- Estado: Acción que está realizando un proceso en un preciso momento.
- Prioridad: Orden en el que se ejcuta un proceso con respecto a otros.
- Contador de programa: Dirección de la siguinete instrucción a realizar de un programa.
- Punteros a memoria: Variable que almacena la dirección de memoria de un objeto.
- Datos de contexto: Datos que están presentes en los registros del procesador cuando el proceso está corriendo.
- Información de estado de E/S: Peticiones de E/S pendientes o dispositivos de E/S asignados a dicho proceso, lista de ficheros en uso por el mismo, entre más acciones relacionadas con E/S.
- Información de auditoría: Cantidad de tiempo del procesador, límites de tiempo, registros contables, entre más.

### Estados del proceso
- Nuevo: Se soilicita al sistema operativo la creación de un proceso. En este estado sus recursos y estrucutras están siendo creadas.
- Preparado: El proceso se encuentra listo para iniciar o continuar su ejecución, aunque necesita ser asignado a un procesador.
- En ejecución: El proceso se encuentra realizando aquello que se le haya asignado hacer en algún procesador.
- Bloqueado: En espera de algún evento para poder continuar su ejecución.
- Terminado: Ejecución del proceso ha sido terminada. A la espera de que sus estrcuturas sean limpiadas por el sistema operativo.
![Alt text](https://sites.google.com/site/materiasisoperativo/_/rsrc/1368848046104/unidad-2-administrador-del-proceso-y-del-procesador/2-2-estados-y-transiciones-de-los-procesos/estados%20de%20procesos.png)

### Ejemplo de un proceso
**Proceso**: Imprimir un archivo de Word.
- Nuevo: En la pestaña de imprimir se presiona el botón Imprimir.
- Preparado: El proceso es admitido y es asignado a un procesador.
- En ejecución: El proceso entra a ejecutarse pero se ve bloqueado al no detectar un dispositivo de E/S.
- Bloqueado: El proceso requiere de que la impresora (dispositivo de E/S) esté conectada.
- Preparado: Una vez la impresora se conecta, el proceso vuelve a ser admitido y llama a ser ejecutado.
- En ejecución: El documento de Word empieza a imprimirse.
- Terminado: El documento es impreso de forma exitosa y el proceso se ve finalizado.

### Interrupciones y planificadores de procesos
**Interrupción**: Señal recibida por el procesador de una computadora que indica que debe interrumpir el curso de ejecución actual y pasar a ejecutar código específico para tratar esta situación.
**Planificador de procesos**: Forma en que se pueden acomodar los procesos para ser ejecutados. Existen varios tipos:
- FCFS (First Come First Served)/FIFO (First In First Out): Ejecución de procesos en orden según su llegada.
- SJF (Shortest Job First): Ejecución prioritaria a los procesos con el menor tiempo asignado.
- Round Robin: Se asigna un tiempo igualitario de ejecución para todos los procesos.
- Planificación por prioridad: Se asigna una prioridad a cada proceso y se ejecutan respecto a esa prioridad.
- Planificación garantizada: Se enfoca en la cantidad de usuarios que debe atender.
- Derivado de MQS (Multiple Queue Scheduling): Una cola de procesos en estado de listos que se divide en varias colas más pequeñas.

## Almacenamiento
### Unidades de almacenamiento
La unidad mínima de almacenamiento es el bit [b]. El bit es simplemente un cero o uno.
El Byte [B] está compuesto por 8 bits y es aproximadamente un caracter.
### Tabla de unidades de almacenamiento
A pesar de que teóricamente las unidades de almacenamiento pueden subir de forma infinita, actualmente no hay capacidad de memoria en existencia que exceda la brecha de los terabytes.
![Alt text](https://i.ytimg.com/vi/yK9fvJ7Mmhg/maxresdefault.jpg)
### Tabla de conversiones de almacenamiento
Para convertir una unidad menor a una mayor se divide entre la cantidad indicada y para convertir una unidad mayor a una menor se multiplica por la cantidad indicada.

![Alt text](https://4.bp.blogspot.com/-TkQXe0rIK9U/WPqd-tb2zNI/AAAAAAAAB0c/ZUtnahEDzCY_7QbGmIZ6Udssld2PJ6XaACLcB/s1600/Unidades.PNG)
### Dispositivos de almacenamiento
- Disco duro
- DVD
- CD
- Memoria USB
- Tarjeta SD
- Disquete

## Jerarquía de memoria
Los usuarios y sobretodo los programadores buscan una memoria muy rápida, muy grande y bajo costo. Sin embargo, al buscar esto, se introduce el siguiente paradigma:
- Muy rápida = Pequeña + cara
- Muy grande = Lenta + barata
- Bajo costo = Grande + lenta

Parece no existir una memoria que cumpla con los tres factores primordiales, por lo que se tiene que buscar un balance entre los tres factores. 
Existe un digrama donde se organizan las memorias en una pirámide poniendo los dispositivos de almacenamiento pequeño, rápidos y caros en la punta y conforme desciende los dispositvos de almacenamiento se vuelven más grandes, lentos y baratos.

![Alt text](https://weblinus.com/wp-content/uploads/2021/02/PiramideMem.jpeg)
## Virtualización de CPU, Virtualización de Memoria, Concurrencia y Persistencia
### Virtualización de CPU
La virtualización del CPU hace referencia a una tecnología que permite la ejecución de varias máquinas virtuales sobre una máquina física con el objetivo de aprovechar al máximo los recursos de un sistema y que su rendimiento sea mayor.
### Virtualización de memoria
Crear una memoria de función compartida mediante una distribución en la red para que los distintos equipos la utilicen. Ofrece ventajas similares al almacenamiento en red.
### Concurrencia
La habilidad de distintas partes de un proceso de ejecutarse en desorden, sin afectar el resultado final, esto debido a que pueden ser ejecutados en múltiples procesadores o en distintos hilos de ejecución.
### Persistencia
Se refiere a la habilidad que tienen los datos de preservar su información de forma permanente.
## Instalación de Ubuntu
### Requerimientos
- Descargar Ubuntu Desktop 20.04 ISO image para arquitectura de x86_64bits
- Descargar aplicación Rufus

### Crear espacio libre en disco duro
- Paso 1: Abrir la terminal y ejecutar el comando diskmgmt.msc para abrir la aplicación de Disk Management.
- Paso 2: Seleccionar la partición que se desea segmentar (normalmente la C:), hacer click derecho y seleccionar la opción Shrink Volume para reducir el tamaño de la partición del disco.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Windows-Disk-Management-Tool.png)
- Paso 3: Asignar la cantidad de MB que se desea asignar a la nueva partición.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Shrink-Windows-Partition.png)
- Paso 4: Tras la asignación de alamcenamiento, aparecerá la nueva partición como "Unallocated" que significa "no asignado".
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/New-Unallocated-Partition.png)
### Instalación y configuración de Ubuntu
- Paso 1: Reiniciar el equipo y presionar la tecla F12, F10 o F2 para iniciar con la instalación de Ubuntu.
- Paso 2: En la primera pantalla, elegir la opción de instalar Ubuntu.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Install-Ubuntu-20.04-Desktop.png)
- Paso 3: En la segunda pantalla elegir la opción de teclado.
- Paso 4: En la siguiente pantalla elegir el tipo de instalación, "Normal" o "Minimal"; se recomienda instalar la opción de "Normal" ya que la opción "Minimal" está más limitada.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Select-Ubuntu-Installation-Type.png)
- Paso 5: En la pantalla siguiente, elegir como tipo de instalación la última opción.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Choose-Ubuntu-Manual-Partition.png)
- Paso 6: En la pantalla de selección del espacio donde se instalará Ubuntu, seleccionar el espacio previamente liberado y presionar el botón de +.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Choose-Free-Space-Partition.png)
- Paso 7: En la ventana emergente, elegir las siguientes opciones en los siguientes recuadros: 
    * Size (Tamaño) = Tamaño de la partción previamente asignada en MB.
    * Type for the new partition (Tipo de la nueva partción) = Primary
    * Location for the new partition (Localización de la nueva partición) = Beginning of this space
    * Use as (Usar como) = EXT4 journaling file system
    * Mount point (Punto de montaje) = /

  Tras llenar estas opciones presionar el botón de OK para regresar a la pantalla anterior.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Create-Root-Ubuntu-Partition.png)
- Paso 8: Seleccionar la ya configurada partición y presionar "Install Now". Aparecerá una pantalla emergente pero solo hay que presionar al botón de continuar.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Partition-Table-Summary.png)
- Paso 9: Seleccionar la región donde uno vive en un mapa para registrar la zona horaria.
- Paso 10: Configurar el nombre de usuario y la contraseña. Al igual que elegir a consideración de cada quien si desea pedir la contraseña o no al iniciar el equipo. Posteriormente iniciará el proceso de instalación.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Create-Ubuntu-User.png)
- Paso 11: Esperar a que se termine la instalación hasta que aparezca una ventana emergente pidiendo reiniciar el equipo.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Ubuntu-Installation-Finishes.png)
- Paso 12: Tras reiniciar el equipo, la pantalla del GNU GRUB debe aparecer y se elige la opción de Ubuntu. De no aparecer el menú GNU GRUB, se debe reinicar el equipo nuevamente y en la BIOS cambiar la prioridad de inicio. Con esto se habrá completado la instalación y configuración de Ubuntu.
![Alt text](https://www.tecmint.com/wp-content/uploads/2018/05/Ubuntu-Grub-Menu.png)
