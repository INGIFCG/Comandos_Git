<h1 ><strong>git init</strong></h1>
<p>Permite iniciar nuestro proyecto en github</p>
<br />
<h1 ><strong>git add<strong></h1>
<br />
<p>Permite agregar nuestros archivos o contenido que deseseemos a una etapa de preparacion antes de hacer un commit o crear una nueva version de nuestros archivos</p>
<p>EJEMPLO:  git add "Nombre del arhcivo a cargar"</p>
<br />
<h1 ><strong>git status<strong></h1>
<br />
<p>Nos permite visalizar los archivos que se desean agregar a la branch</p>
<br />
<h1 ><strong>git -m commit "Texto"<strong></h1>
<p>Permite confirmar una nueva version del codigo que esta a la espera de ser commiteados</p>
<br />
<h1 ><strong>git add .<strong></h1>
<p>Permite cargar todos los archivos en el proyecto que no han sido traqueados o cargados</p>
<br />
<h1 ><strong>git add --patch<strong></h1>
<p>Permite cargar o actualizar las partes modificadas de un archivo, en este caso un ejemplo seria <strong> add index.php --patch</strong>, esto unicamente mostrara e indicara que si se desea cargar las lineas o las funciones modificadas del proyecto a la rama principal.</p>
<br />
<h1>git diff<strong><strong></h1>
<p>nos permite visualizar las diferencias entre el archivo añadido entre el ultimo commit y el que se ha modificado actualmente</p>
<br />
<h1><strong>git log<strong></h1>
<p>Permite visualizar el historial de los commits en nuestro proyecto </p>
<br />
<h1><strong>git log --onleline<strong></h1>
<p>nos permite tener una vista mas simplificada que la de <strong>git log</strong>, mostrandonos a demas el hash vinculado a cada commit</p>
<br />
<h1><strong>git log --stat<strong></h1>
<p>Nos permite visualizar cuantos han sido los cambios, en este caso serial las insersiones o eliminaciones de lineas de codigos en cada uno de nuestros commit </p>
<br />
<h1><strong>git log -p<strong></h1>
<p>Nos permite visualizar el codigo entre cada commit de lo que se modifico en nuestro proyecto</p>
<br />
<h1><strong>git branch<strong></h1>
<p>Nos permite guardar o crear una nueva rama, de la cual se desenlace de la rama principal para hacer pruebas o verificaciones en el codigo antes de ser cargada a la rama principal</p>
<p>Ejemplo para crear una nueva rama:
git branch <strong>Nombre de la nueva rama</strong></p>
<br />
<h1><strong>git checkout<strong></h1>
<p>Nos permite hacer el cambio hacia la nueva rama creada</p>
<p>Ejemplo:
git checkout<strong>nuevaRama</strong><p>
<br />
<h1><strong>git checkout -b<strong></h1>
<p>Es otra forma de crear ramas de una forma mas sencilla, a lo cual se puede crear la nueva rama y cambiar a la misma en el mismo momento de crearla</p>
<p>ejemplo <strong>git checkout -b nuevaRama</strong>, lo que hace esto es crear una nueva rama llamada nuevaRama y automaticamente despues de crearla se mueve a dicha rama sin necesidad de otro comando </p>
<br />
<h1><strong>git merge<strong></h1>
<p>Nos pemite combinar los commit o los  cambio que se han echo entre 2 ramas, dando como resultado una sola rama en la cual contendra todos los cambios que nosotros solicitemos,para hacer esto es necesario que no tengamos ningun archivo por hacerle commit o cargarlo a la rama, en ninguna de ambas ramas.<br /> 
Para esto es necesari que estemos principlamnete en la rama donde combinaremos ambas ramas</p>

<p>ejemplo <br />
<strong>git merge nombreDeLaRamaAcombinar</strong> 
</p>
<br />
<h1><strong>Comandos para trabajar con repositorios remotos<strong></h1>
<br />
<br />
<br />
<h1><strong>git remote<strong></h1>
<p>Al momento de crear un nuevo repositorio en github nos daran la url del repositorio en este caso para si se desea agregar un nuevo repositorio remoto se debera crear el repositorio en git, seguidamente se debera colocar el siguiete comando</p>
<h2><strong>git remote add origin <strong>url dada por githun</strong><strong></h2>
<p>Una ves echo esto nos asignara el respositorio como origin</p>
<br />
<h1><strong>git remote -v<strong></h1>
<p>Nos permite visualizar mas detalle del repositorio a la cual se mostrara las opciones fetch y push</p>
<br />
<h1><strong>git push<strong></h1>
<p>nos permitira cargar o enviar los datos a la rama principal</p>
<br />
<p>PARA insertar los datos en el respotirio esto nos solicitara lo siguiente: <br /> 
git push <strong>NombreDeLaRamaAsubir</strong> main</p>
<br />
<h1><strong>git pull remotoDondeSeDescargaraLaINFO(por defecto sera origin) ramaADescargar(por defecto puede ser main)<strong></h1>
<p>nos permite descargar el repositorio</p>
<br />
<h1><strong>git fetch</h1>
<p>nos permite descargar el contenido del repositorio, la diferencia entre git pull y git fetch es git fetch va a descargar el contenido pero no le aplicara un merge, esto quiere decir que podremos acceder a estos cambios sin mezclarlo al proyecto principal</p>
<br />
<h1>git clone<strong><strong></h1>
<p>nos permite clonar o descargar un proyecto que no necesariamente es de nuestra propiedad, esto se hace de la siguiente manera</p><br />
<p>git clone (url del proyecto remoto)</p>
<br />
<h1><strong>git log --oneline --graph --all<strong></h1>
<p>nos muestra todos los pull requests añadidos en el proyecto a lo largo del tiempo</p>
<br />
<h1><strong>git stash<strong></h1>
<p>Nos permite guardar de forma temporal una porcion de nuestro codigo sin la necesidad de hacer un commit</p>
<br />
<h1><strong>git stash pop<strong></h1>
<p>nos permite regresar los cambios aplicados anteriormente en main</p>
<br />
<h1><strong>git checkout (hash)<strong></h1>
<p>nos permite navegar dentro de los commits para validar a fondo los cambios ejecutados a lo largo de dichos commits</p>
<br />
<h1><strong>git reverse<strong></h1>
<p>nos permite deshacer o revertir un commit, esto tomara el ultimo commit y hara los cambios inversos a lo echo en dicho commit, en este caso lo que ara es revertirlo y agregar los trozos de codigo que fueron eliminados </p>
<br />
<h1><strong>git reset --hard<strong></h1>
<p>Es otra forma de revertir un commit </p>
<p>Ejemplo <br /> 
git reset --hard (hash del commit al que se quiere revertir);
</p>
<p>No es recomendable a la hora de tener un repositorio central o cincronizados</p>
<br />
<h1><strong>git commit --amend<strong></h1>
<p>Nos permite agregar una modificacion a nuestro ultimo commit echo en el proyecto, esto nos ayuda por si nos olviamos en modificar algo de ultimo momento</p>
<br />
<h1><strong>git rebase<strong></h1>
<p>nos permite hacer un merche con la particularidad de tomar todos los commit que se tengan en una rama y nos la coloca en otra rama.</p>
<br />
<h1><strong><strong></h1>
<p></p>
<br />
<h1><strong><strong></h1>
<p></p>
<br />
<h1><strong><strong></h1>
<p></p>