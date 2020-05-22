# proyecto_motor
Muestra la información de un motor de corriente alterna, dados los datos de un servidor establecido. Dicho proyecto se actuliza 
periodicamente mediante un push button.

#Procedimiento de uso
Para realizar el uso del proyecto, es necesario seguir los siguientes pasos:
  1. Guardar la carpeta "Tercio3" en la ruta /home/alse/Documents
  2. Inicializar el archivo UIproyeto.pro mediante el QT CREATOR.
  3. Compilar y ejecutar el archivo dentro el programa.
  4. Disfrutar de su uso.
  
#Comentarios y soluciones a errores:
En dado caso de presentarse algún error de inicialización dentro del proyecto mediante el QT CREATOR, primero realizar dentro 
de la consola la compilación y ejecución del código "UDPEchoClient.c" teniendo en cuenta como prioridad la CONEXIÓN
A INTERNET dentro de la máquina a utilizar. La ejecución dentro de consola es de la siguiente manera:

  1. cd home/alse/Documents/Tercio3/version7  //Cambia el directorio base, al directorio donde se encuentra el proyecto
  2. gcc UDPEchoClient.c -o UDPEchoClient.bin //Compila el proyecto en caso de error
  3. ./UDPEchoClient.bin (ip del servidor del motor) (Carné del usuario válido) (Puerto de comunicación) //Ejecuta el proceso mediante los      argumentos de entrada.
  4. Verificar la validación de la comunicación y los archivos recibidos del servidor, dicha validación se verá dentro de un mensaje
     el cúal dirá "se guardaron los datos del motor".
  5. Verificar la creación del archivo "/home/alse/Documents/Tercio3/version7/datos_motor.txt"
  
Realizada dicha ejecución se vuelve a compilar y ejecutar el código dentro del QT CREATOR, y verificar el funcionamiento
