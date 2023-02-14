# Docker + python

---

# Creamos el contenedor sencillo python

`$ docker run -it --rm --name my-running-script -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python your-daemon-or-script.py`

`docker`es el comando base.

`Run` es para crear el cotnenedor.

`-it` para interactuar con la terminal.

`-rm` borra el contendor cunado finaliza la acción.

`--name` ponerle nombre.

`-v` define el mapeo del volumen localmente.

- `$PWD` el directorio donde estamos.

- `:/usr/src/myapp` el directorio dentro del contenedor.

`-w` el directorio de trabajo.

`python:3` nombre de la imagen.

`python your-daemon-or-script.py` es el comando para ejecutar dentro del contenedor.

