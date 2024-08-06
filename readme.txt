
INSTRUCCIONES PARA EL CORRECTO DESPLIEGUE DE LA APLICACIÓN

NOTA:
-Es necesario instalar Python 3.11.3 para evitar problemas de incompatibilidad con los paquetes.
-En Linux se accede a la carpeta /bin para usar Python.
-Es necesario instalar node y npm (versión igual o superior a 10.2.4).
-Ejecutar el comando "npm i" para instalar los datos relacionados con Vite.


1. Las librerías necesarias para la ejecución de los archivos de Python están desinstaladas para ahorrar espacio.
    -Instalar librerías: cd doodleAdoodle -> bin/python -m pip install -r requirements.txt    
    -Desinstalar librerías: cd doodleAdoodle -> bin/python -m pip uninstall -r requirements.txt -y



2. Desplegar cada uno de los servidores con los siguientes comandos:
    -cd doodleAdoodle -> bin/python app/src/model/CNNServer.py
    -cd doodleAdoodle -> bin/python app/src/model/dataBaseServer.py
    -cd doodleAdoodle/app -> npm run dev -- --host
    -cd doodleAdoodle -> node app/src/model/socketIOServer.js



3. Si hay algún error con la ip, cambiar de forma manual en los siguientes archivos
y desplegar los servidores:
    -doodleAdoodle/app/src/model/CNNServer.py: Cambiar ip en la linea 79.
    -doodleAdoodle/app/src/model/dataBaseServer.py: Cambiar ip en la linea 450.
    -doodleAdoodle/app/src/view/main.jsx: Cambiar ip en la linea 9.
