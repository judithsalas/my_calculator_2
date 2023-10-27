**Proyecto calculadora 2**

Para la realización del proyecto se han seguido los siguientes pasos:

En primer lugar, se creó un repositorio público en github nombrado *my_calculator_2*, donde se añadió el clon del repositorio my_calculator 
y se realizaron una serie de cambios.

A continuación, se introdujeron en git bash los comandos pertinentes:
 
Comenzando por **git git clone https://github.com/my_calculator   my_calculator_2**, a partir de él clonamos en "my_calculator_2", el repositorio my_calculator.
A continuación, se creó una rama que partiera del primer commit nombrado como <x^3 button>, con los commits **git log --oneline**, por el cual copiamos el id del 
commit de interés y lo reservamos para introducirlo en el siguiente comando que fue el encargado de crear nuestra nueva rama  **git checkout -b ops <id_de_commit>** 

Posteriormente, en la nueva rama que se creó nombrada como "ops", se añadieron los botones de x^2 y 1/x, introduciendo primero el código de la x^2 en el 
archivo index.html. Una vez se añadió el código se guardaron los cambios y se ejecutaron los comandos **git add index.html** y **git commit -m "mensaje de interés según el botón"**

Después, se integró la rama ops en la rama master a partir del commit "1/x button", donde se copió el id del commit para utilizarlo posteriormente para hacer el rabase. Se utilizó **git log --oneline** para conocer el id del commit.

Se resolvieron los conflictos desde el archivo index.html de forma manual, se añadieron los cambios con **git add .**, y **con git rebase --continue** se integró la rama ops introduciendo los cambios en el índice y se añadió un commit.

Una vez se resolvieron todos los conflictos y el commit fue generado ya se efectuó el rebase se realizó el push llevando los cambios al repositorio remoto.
