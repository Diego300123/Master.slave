# Ejercicios de Vagrant y Configuración de DNS

Este repositorio contiene una serie de ejercicios para configurar máquinas virtuales y un sistema de nombres de dominio (DNS) con Vagrant.

---

## Exercice 1

Vamos a crear los archivos `Vagrantfile` y `.gitignore`. Configuraremos `.gitignore` para ignorar cambios en los archivos `.vagrant` y en archivos de respaldo según lo solicitado en el ejercicio.

Finalmente, crearemos también el archivo `README.md` para documentar los ejercicios realizados y el archivo `LICENSE` con una licencia de mi elección.

---

## Exercice 2

Incorporamos las instrucciones necesarias en el `Vagrantfile` para crear dos máquinas virtuales (venus y tierra) con sus respectivas direcciones IP.

Finalmente, ejecutamos `vagrant up` para levantar las máquinas virtuales.

---

## Exercice 3

### Configuraciones en los archivos

1. Para las secciones 1, 2 y 3, configuramos el archivo `named.conf.options`. Para ello, copiamos el archivo fuera de la máquina, lo modificamos y luego lo volvemos a copiar dentro de la máquina.
2. En la sección 4, modificamos ciertos archivos en la máquina `tierra` para configurarla como un sistema maestro.
3. En la sección 5, modificamos algunos archivos en la máquina `venus` para configurarla como un sistema esclavo.
4. En la sección 6, configuramos la sección "Negative Cache TTL" en el archivo `db.system.test`.
5. Para la sección 7, configuramos una sección en el archivo `named.conf.options` para que las consultas no autorizadas se redirijan a una IP específica.
6. En la sección 8, configuramos el archivo `db.sistema.test` para añadir los alias solicitados en el ejercicio.
7. Para las secciones 9 y 10, configuramos el archivo `db.sistema.test` para añadir a `marte` como el sistema de correo, según las instrucciones del ejercicio.
