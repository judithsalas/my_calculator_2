#Proyecto calculadora 2#
Para la realización del proyecto se han seguido los siguientes pasos:

En primer lugar, se creó un repositorio público en github nombrado *my_calculator_2*, donde se añadió el clon del repositorio my_calculator 
y se realizaron una serie de cambios.

A continuación, se introdujeron en git bash los comandos pertinentes:
 
Comenzando por **git git clone https://github.com/my_calculator   my_calculator_2**, a partir de él clonamos en "my_calculator_2", el repositorio my_calculator.
A continuación, se creó una rama que partiera del primer commit nombrado como <x^3 button>, con los commits **git log --oneline**, por el cual copiamos el id del 
commit de interés y lo reservamos para introducirlo en el siguiente comando que fue el encargado de crear nuestra nueva rama  **git checkout -b ops <id_de_commit>** 

Posteriormente, la nueva rama que se creó nombrada como "ops", 
tras este paso, se asignó el repositorio remoto que habíamos creado en Git hub con ** git remote add origin https://github.com/<mi usuario de github>/my_calculator.git**

Después, se creó un archivo html al que hemos nombrado como index.html **nano index.html**, este fichero contiene una calculadora web con un botón para hayar el cubo del número introducido 
Una vez completado el fichero, se añadió en el índice **git add index.html** y se efectuó el primer commit en la rama master con **git commit -m "x^3 button"**. 
Para comprobar el listado de los commits se utilizó **git log --oneline**.

Tras el primer commit, se hizo un segundo en la misma rama en la que se estaba trabajando, la rama main. 
Este segundo commit consistio en añadir a la calculadora un segundo botón(elemento HTML <button ..>)
que eleve un número a la cuarta potencia (x^4)

Para llevarlo a cabo se modificó el fichero index.html **nano index.html**, y se cambió el código añadiendo el botón nuevo (x^4)
Se registraron los cambios en el índice **git add index.html** y  se realizó el segundo commit **git commit -m "x^4 button"**.

El último paso fue llevar los cambios al repositorio remoto con **git push**
