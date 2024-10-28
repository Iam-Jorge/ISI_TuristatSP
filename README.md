# TuriStatSP
Repositorio del laboratorio de Integración de Sistemas de Información

El usuario debe descargarse flask_cors, flask, requests, beautifulsoup4, sqlite3, sqlitebrowser, matplotlib, numpy y pytest.

pip install matplotlib requests numpy beautifulsoup4 flask flask_cors pytest

**Si da problemas tkinter, instalar mediante "pip install tk" (no debería de dar ya que esta librería viene con python preinstalada)**

Sqlite3 en: https://www.sqlite.org/download.html
Sqlitebrowser: https://sqlitebrowser.org/dl/

## Inicialización de la aplicación sin docker
Primero debe de estar el servidor Flask encendido, para que la aplicación funcione correctamente.
1. Nos metemos en la carpeta persistencia desde la terminal (y dependiendo de donde lo guardes). "cd isi-TuriStatSP/persistencia"
2. Desde la terminal, estamos situados en persistencia y tenemos que iniciar el servidor mediante “obtenerDatosJson.py”. Por lo que escribimos “export FLASK_APP=obtenerDatosJson” y luego “flask run”. 
3. Una vez tenemos esto, ejecutamos el “manager.py” que está en "isi-TuriStatSP"

## Inicialización de la aplicación con docker
Dentro de la carpeta del proyecto ("cd isi-TuriStatSP"), hay que ejecutar las siguientes instrucciones:
1. "docker build -f Dockerfile -t isi-turistatsp:latest ." (solamente para crear la imagen en tu ordenador, la primera vez).
2. "docker run -p 5000:5000 -d isi-turistatsp" (Una vez que lo has puesto una vez, puedes pausar o iniciarlo de nuevo desde la interfaz de Docker Desktop).
Y ya una vez realizado, puedes ejecutar el manager.py directamente.


