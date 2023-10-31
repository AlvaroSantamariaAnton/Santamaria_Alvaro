Nombre del alumno: Álvaro Santamaría Antón
Link al repositorio de GitHub: https://github.com/AlvaroSantamariaAnton/Santamaria_Alvaro.git

Respuestas al examen:

1º Un Pull Request consiste en enviar una solicitud a un repositorio de GitHub para que el propietario de dicho repositorio integre los cambios que tu has hecho en una copia de su repositorio, el cual
   se ha creado mediante un Fork. De este modo el propietario pordrá aceptar o denegar el pull request con el objetivo de integrar o denegar los cambios que tu has hecho, respectivamente.

2º Un Merge Conflict es un conflicto que surge al hacer un merge (fusionar dos ramas), esta integración puede tener algún conflicto, por ejemplo, que haya dos líneas con el mismo contenido. 
   Para solucionar este conflicto entraría al fichero en cuestión mediante el comando "nano" y lo arreglaría manualmente, quitando las cosas innecesarias y ajustando todo a la perfección, luego 
   mediante el comando "git merge --continue" terminaría el merge.
   
3º Primero nos situamos en la rama "examen_parcial" mediante el comando "git switch examen_parcial", posteriormente mediante el comando "git merge examen_parcial main" integramos los cambios de main 
   en la rama examen_parcial, si hubiese algún conflicto lo solucionaría con el editor y terminaría la integración con "git merge --continue", después me cambio a la rama main mediante "git switch main" y 
   mediante el comando "git merge main examen_parcial" integro los cambios de la rama examen_parcial en la rama main, si hubiese conflictos nuevamente se resolverían manualmente y finalizo
   con "git merge --continue".

4º Mediante el comando "git checkout <commit>" podría mantener los cambios en el index pero volver al commit que yo quiera.

5º Para realizar un fork debemos ir a un repositorio de GitHub que no nos pertenezca y cerca de la esquina superior derecha encontraremos un botón llamado "Fork", para hacer el fork hacemos clic en 
   el botón y volvemos a confimar para copiar el repositorio en nuestra cuenta. Esto se utiliza normalmente para copiar un repositorio de GitHub a nuestra cuenta con el objetivo de contribuir.

6º a) Desde el directorio raíz (\) haría el comando "cd Universidad" para entrar en ese directorio, posteriormente haría "cd UAX" para entrar en dicho directorio y finalmente mediante el comando "ls" 
      confirmaría que me encuentro en el directorio en el que está el fichero "archivo.txt". Opcionalmente podría usar el comando "cd Universidad/Uax/" desde el directorio raíz y de esa manera llegar 
      con un solo comando. Esto sería un ejemplo de ruta absoluta absoluta, ya que representa la ruta completa, parte del directorio raíz hasta llegar al fichero deseado.
      
   b) Usaría el comando "cd UAX" para acceder al repositorio que contiene el "archivo.txt". Esto sería un ejemplo de ruta relativa, ya que solo representa una parte de la ruta, teniendo en cuenta el 
      directorio desde el que partimos.

7º 1) b) git clone
   2) a) git branch
   3) c) git checkout
   4) b) git add
   5) b) git commit
   6) b) git push
   7) c) git pull
   8) d) git merge
   9) a) git reset --hard
   10) c) git log

8º Para empezar decidiría cual de las ramas va a integrarse antes, por ejemplo, primero se integrará la rama "matemáticas" y posteriormente la rama "Diseño UX". Si aún no estoy en la rama main, entro 
   a ella mediante el comando "git switch main", posteriormente mediante el comando "git merge main matemáticas" integro los cambios de matemáticas en main, si surge algún conflicto los resuelvo 
   manualmente con el editor y termino la integración con "git merge --continue", una vez acabada la integración verifico la integridad de los ficheros de main y que todo funcione correctamente, podría 
   hacer el comando "git status" para verficar el estado de los archivos y por último mediante el comando "git commit -m "merge matemáticas" realizo la instantánea. Posteriormente, para integrar la 
   rama "Diseño UX" repetiría el proceso anterior, "git merge main Diseño UX", resolvería conflictos si hubiese, "git merge --continue", verifico la inetgridad de los archivos de main y verifico que 
   todo funciona bien, tanto la parte de main como la añadida recientemente parte de matemáticas, finalmente "git status" para revisar el estado de los ficheros y "git commit -m "merge Diseño UX" 
   para hacer la instantánea.
   
9º C) Añadiste el botón "x^4" al archivo "index.html" en tu repositorio local, creaste un commit con los cambios y luego subiste el repositorio local al remoto en la rama principal (master).      
