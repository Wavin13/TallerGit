Taller git
Navegué al directorio home: Empecé utilizando el comando cd ~ para volver a mi directorio personal.
Fui al escritorio: Luego, cambié al directorio de mi escritorio con cd desktop.
Entré en la carpeta de programación: A continuación, accedí a la carpeta de programación utilizando cd programacion.
Inicialicé un nuevo repositorio Git: Usé git init TallerGit para crear un nuevo repositorio vacío llamado TallerGit.
Configuré mi nombre en Git: Configuré mi nombre de usuario global con el comando git config --global user.name "Nelson Holguin".
Configuré mi correo electrónico en Git: Luego, establecí mi correo electrónico global con git config --global user.email "nelson.holguin@correounivalle.edu.co".
Intenté agregar un repositorio remoto: Intenté añadir un remoto con git remote add origin https://github.com/Wavin13/TallerGit.git, pero recibí un error porque no estaba en un repositorio Git.
Entré en la carpeta del repositorio: Cambié al directorio TallerGit usando cd TallerGit.
Agregué el repositorio remoto correctamente: Ahora, volví a ejecutar el comando git remote add origin https://github.com/Wavin13/TallerGit.git, y esta vez funcionó.
Creé una nueva rama: Utilicé git checkout -b feature para crear y cambiar a una nueva rama llamada feature.
Creé un archivo de texto: Escribí "Texto inicial" en un archivo llamado archivo.txt usando echo "Texto inicial" > archivo.txt.
Agregué el archivo al área de preparación: Utilicé git add archivo.txt para añadir el archivo al área de preparación.
Hice el primer commit: Realicé mi primer commit con git commit -m "Commit inicial".
Agregué más texto al archivo: Añadí más texto al archivo usando echo "Texto agregado en feature" >> archivo.txt.
Hice el segundo commit: Realicé el segundo commit con git commit -am "Segundo commit en feature".
Agregué más texto nuevamente: Añadí otro texto con echo "Texto agregado por tercera vez" >> archivo.txt.
Intenté hacer un commit, pero no se registraron cambios: Al intentar hacer un commit con git commit -m "Tercer commit en feature", Git me indicó que había cambios no preparados.
Hice el tercer commit correctamente: Luego utilicé git commit -am "Tercer commit en feature" para registrar esos cambios.
Intenté cambiar a la rama master, pero no existía: Al usar git checkout master, recibí un error indicando que no había un branch master.
Verifiqué las ramas existentes: Utilicé git branch y confirmé que solo existía la rama feature.
Creé la rama master: Después, ejecuté git checkout -b master para crear la nueva rama master.
Verifiqué las ramas nuevamente: Usé git branch para asegurarme de que ahora tenía ambas ramas, feature y master.
Hice un merge de la rama feature: Intenté fusionar feature en master usando git merge feature, pero Git me dijo que ya estaba al día.
Hice un reset a un commit anterior: Utilicé git reset --hard HEAD~1 para retroceder un commit en la rama master.
Hice un rebase de la rama feature: Ejecuté git rebase feature para aplicar los cambios de feature en master.
Creé una nueva rama hotfix: Luego, creé una nueva rama llamada hotfix usando git checkout -b hotfix.
Agregué una corrección urgente: Escribí "Correcion urgente" en archivo.txt y lo comprometí con git commit -am "Hotfix".
Regresé a la rama master: Usé git checkout master para volver a la rama master.
Hice cherry-pick de hotfix: Apliqué los cambios de la rama hotfix en master con git cherry-pick hotfix.
Volví a la rama feature: Cambié nuevamente a la rama feature con git checkout feature.
Creé un archivo para provocar un conflicto: Usé echo "Cambio en feature" > conflicto.txt para crear un nuevo archivo.
Intenté hacer un commit, pero no se registró: Al ejecutar git commit -am "Cambio en feature", Git me dijo que había archivos no rastreados.
Regresé a la rama master: Cambié a la rama master con git checkout master.
Agregué otro archivo que provocó el conflicto: Escribí "Cambio en master" en conflicto.txt.
Intenté hacer un commit en master, pero no se registró: Al hacer git commit -am "Cambio en maste", Git nuevamente indicó que había archivos no rastreados.
Agregué el archivo conflicto.txt a master: Usé git add conflicto.txt para agregarlo al área de preparación.
Hice el commit en master: Realicé el commit con git commit -am "Cambio en master".
Intenté hacer un merge de feature en master: Ejecuté git merge feature, pero Git me informó que ya estaba al día.
Verifiqué el estado del repositorio: Usé git reflog para revisar el historial de cambios.
Volví a la rama feature: Usé git checkout feature para cambiar de vuelta a la rama feature.
Creé el archivo conflicto.txt nuevamente: Escribí "Cambio en feature" en conflicto.txt.
Intenté hacer el commit de nuevo, pero no se registró: Ejecuté git commit -am "Cambio en feature", pero Git me indicó que había archivos no rastreados.
Agregué conflicto.txt a la rama feature: Utilicé git add conflicto.txt para agregarlo.
Hice el commit de los cambios en feature: Realicé el commit con git commit -am "Cambio en feature".
Regresé a la rama master una vez más: Cambié a master usando git checkout master.
Hice un cambio en conflicto.txt nuevamente: Escribí "Cambio en master" en conflicto.txt.
Intenté hacer el commit en master: Al ejecutar git commit -am "Cambio en master", Git me dijo que había archivos no rastreados.
Agregué conflicto.txt a master: Usé git add conflicto.txt para agregarlo.
Hice el commit en master: Realicé el commit con git commit -am "Cambio en master".
Intenté hacer el merge de feature en master nuevamente: Ejecuté git merge feature, pero me encontré con un conflicto de merge.
Verifiqué el estado del merge: Usé git status para ver que tenía rutas no fusionadas.
Resolví el conflicto: Registré la resolución del conflicto usando git commit -am "El conflicto lo resolvi juntando todo en una sola linea".
Verifiqué que no había cambios pendientes: Ejecuté git status y vi que el árbol de trabajo estaba limpio.
Intenté hacer un push a la rama master: Al usar git push -u origin, me informó que no había una rama upstream configurada.
Verifiqué los remotos configurados: Usé git remote -v para ver las URL de los remotos.
Hice el push de la rama master: Finalmente, ejecuté git push -u origin master para subir mis cambios al repositorio en GitHub.
