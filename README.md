# Bienvenidos a GitCommands!!

:unlock: Comandos Git aprendidos en Platzi :fire: :computer: :rocket:


> **Siéntase libre de compartir su conocimiento en este proyecto**.

#

- **git init**                                    -- Se utiliza inicializar git, se debe de realizar dentro del                directorio raíz del proyecto.

- **git Add .**                                -- Se agregan todos los cambios de todos los archivos en memoria ram para ser rastreados o identificados. Notar que después de "add" va un "espacio" y luego "punto" .

- **git add nombre del archivo**                   -- Se realiza para agregar solo un archivo a staging.

- **git log nombre del archivo**                   -- Se realiza para ver los cambios realizados con un archivo específico a través de los commit, también se pueden ver los id de cada commit.

- **git diff id commit id commit**                 -- Se utiliza para visualizar los cambios entre 2 versiones de commit, se recomienda colocar el id del commit más viejo primero y el id del                                                 commit mas reciente de segundo, para encontrar los id se utiliza el comando git log. En rojo se identifica el inicio de los cambios o texto cambiado y en verde las adiciones o diferencias con respecto al segundo id de commit.

- **Clear**                                        -- Limpia la terminal de comandos .

- **Cat nombre del archivo**                       -- Se utiliza para ver el contenido del archivo.

- **Code**                                         -- Se utiliza para abrir/ejecutar Studio Code.

- **code nombre del archivo**                      -- Se utiliza para abrir un archivo específico con Studio Code .

- **history**                                      -- Se utiliza para ver el historial de comandos escritos .anteriormente

- **git version**                                  -- Ver la versión de git instalada.

- **ls**                                           -- Ver el contenido disponible dentro de la carpeta en la que se encuentra actualmente.

- **ls - al**                                      -- Se utiliza para ver todo tipo de archivos, incluso los de atributo oculto.

- **git status**                                   -- Se utiliza para ver el estado del directorio sobre el que se declaró "git init". Con este comando podemos saber que cambios han sido agregados al staging y cuales ya están en staging listos para ser inmortalizados a través de un commit.

- **git - rm --cached nombre del archivo**         -- Se utiliza para borrar un cambio de la ram o el staging una vez que haya sido agregado mediante el método "add".

- **git config --list**                            -- Se utiliza para ver la configuración actual en git.

- **git config**                                   -- Se utiliza para mostrar todos las funciones disponibles con dicho comando.

- **git config --global user.name "nombre"**       -- Se utiliza para asignar un nombre de usuario a la configuración de git, debe de ir dentro de las comillas.

- **git config --global user.email "correo"**      -- Se utiliza para asignar una dirección de correo a la configuración de git, debe de ir en comillas.

- **git config --list --show-origin**              -- Se utiliza para identificar las rutas en las que se hospedan los archivos de configuración de git.

- **git commit -m "mensaje explicativo"**          -- Se utiliza para inmortalizar los cambios al repositorio, siempre debe de existir un mensaje que explique los cambios, **siempre**. El mensaje va dentro de las comillas.

- **git commit**                                   -- Al no declarar un mensaje para respaldar los cambios, Git automáticamente abre el editor de texto VIM; y exige agregar una nota que explique el cambio.  Presionamos la tecla "i" para escribir el mensaje y una vez terminado presionamos esc+shift+z+z  para guardar los cambios y salir de VIM.

- **git show nombre del archivo**                  -- Se utiliza para ver los cambios más recientes dentro del archivo, color blanco es lo que estaba anteriormente, color rojo indica el inicio                                                 del cambio y el color verde son los cambios o texto agregado en el último cambio.

- **git reset id del commit --hard**               -- Borra todos los archivos o cambios realizados desde ese commit hasta la rama master, --soft es un poco mas seguro ya que no borra el                                                 contenido existente en staging.

- **git diff**                                     -- Con este comando es posible ver las diferencias entre el último commit y las actualizaciones o cambios realizados. Aclarar que los cambios no necesariamente deben de estar en staging para poder utilizar este comando.

- **git restore nombre del archivo**               -- Se utiliza para quitar un cambio del staging antes de que el mismo sea cargado al repositorio a través de commit.

- **git log --stat**                               -- Es posible ver a mayor detalle los cambios realizados en cada commit, se ven la cantidad de bits agregados o eliminados.

- **git checkout id de commit nombre del archivo** -- checkout se utiliza para ver archivos específicos de un commit id específicos.

- **git checkout master nombre del archivo**       -- Se utiliza para visualizar el estado actual de un archivo específico en la rama principal o rama master; se utiliza para restaurar los cambios del archivo                                                 en local después de haber visualizado el estado del mismo en alguno de los commit anteriores.

- **git checkout nombre de la rama**               -- Se utiliza para desplazarse entre las diferentes ramas existentes.

- **Head**                                         -- Es un indicador de la rama/commit en el que se encuentra. No es un comando :stuck_out_tongue_closed_eyes:

- **git branch nombre de la nueva rama**           -- Con este comando se crea una nueva rama, automáticamente clona la rama en la que se encuentra actualmente al ejecutar el comando.

- **git commit -am "mensaje"**                     -- Se utiliza para cargar en el staging los cambios realizados y en el repositorio a la vez. Solamente funciona con archivos pre-existentes en el repositorio, por lo que si se tratan de archivos completamente nuevos hay que seguir los pasos por separado, utilizando add y commit.

- **git branch**                                   -- Se utiliza para ver las ramas existentes en el repositorio.

- **git merge nombre de la rama secundaria -m "mensaje de referencia"**      -- Este comando se utiliza para unir los 2 últimos commit realizados en cada rama, es importante decidir                                                                             cual rama continuará siendo la principal; usualmente se deja como principal la rama master. Una vez decidido cual rama será la principal hay que posicionarse en ella y luego escribir este comando de forma que el nuevo commit unificado se creará sobre la rama principal seleccionada.

- **git remote add origin link del repositorio en Github**                   -- Esta línea debe de hacerse desde la rama master o rama en la que yace el último commit actualizado. Antes de                                                                           correr este comando se debe de crear un repositorio en GitHub y copiar el URL. Eventualmente hay que hacer un pull (--allow-unrelated-histories) y luego un push para colocar todo el proyecto en el repositorio web.

- **git remote -v**                               -- Se utiliza para ver los URL de los sitios remotos configurados.

- **git pull origin nombre de la rama --allow-unrelated-histories**          -- Cuando se crea un repositorio desde cero en github con el archivo readme el mismo se toma en cuenta como un commit, y al tener nuestro proyecto en disco con sus propios commits se generan unrelated histories o commits, es por ello que el primer pull request se debe de realizar con este comando, de forma que ambos proyectos se puedan sincronizar correctamente.

- **git push origin nombre de la rama(usualmente master)**                   -- Con este comando se envía toda la información alojada en local al repositorio. 

- **pwd**                                         -- Se utiliza para ver en la ruta en la que estamos.

- **git config -l**                              -- Comando para ver la configuración actual de git en el ordenador.

- **ssh-keygen -t rsa -b 4096 -C "correo electrónico de la cuenta en github"**  --  Con este comando se crean las llaves públicas y privadas para establecer una conexión ssh con GitHub. Tener en cuenta que el número "4096" puede ser reemplazado por cualquier parámetro de encriptación que se desee. Este comando debe de ejecutarse en home, la forma de acceder a él es mediante el comando cd. Una vez creadas las llaves públicas y privadas, las mismas se alojarán en C:User/Users/ .ssh, esto para Windows.

- **eval $(ssh-agent -s)**                        -- Se utiliza para determinar si ssh está corriendo en el ordenador y bajo que número de proceso está identificado el mismo. Este comando debe de                                                hacerse antes de agregar las llaves privadas o públicas.

- **ssh-add ruta de la llave que desea agregarse**                           --  Una vez verificado que ssh está corriendo en el ordenador se procede a agregar la llave, es imperativo saber la                                                                            ruta de la llave que se desea agregar, de preferencia este comando debe de correrse en home. Recordar que las                                                                            llaves son a nivel de usuario y no de repositorio.

- **git remote set-url origin dirección web o ssh**         -- Este comando se utiliza para reemplazar el url existente en remote, puede ser en formato de https o ssh, origin es simplemente una variable por default que se asigna para fetch y push, pero la misma puede ser cambiada a placer, para estar seguros siempre se debe                                                          confirmar la info con *remote -v* antes de realizar el cambio

**Nota importante:** *ANTES DE REALIZAR UN PUSH, SIEMPRE ES PRUDENTE REALIZAR UN PULL, DE FORMA QUE LA INFO ESTE ACTUALIZADA Y SE GARANTICE LA CONEXIÓN.*

- **git log --all**                            -                      -- Se utiliza para ver todos los commits sin excepción, es una manera más robusta.

- **git log --all --graph**                                           -- Se aprecia de una manera más gráfica el historial de los commit, así como las ramas creadas y sus respectivos commits.

- **git log --all --graph --decorate --oneline**                      -- Resume y decora aún mas el historial de commits, hash de commits y sus respectivas ramas. Sin duda este comando hace más entendible la historia de commits de nuestros proyectos.

- **alias nombre del alias="comando que se desea resumir a través del alias"**            -- Con alias se resumen líneas de comando extensas en palabras simples, ejemplo *arbolito*.

- **git tag -a nombre de la versión -m "mensaje" id del commit** -- Con este comando somos capaces de agregar un tag al commit deseado, usualmente se usa para la asignación                                                                                    de versiones a nuestro proyecto, muy útil ya que es fácil de entender estando desde GitHub.

- **git tag**                                                    --- Se utiliza para ver las versiones, tags existentes.

- **git show-ref --tags**                                        -- Se utiliza para ver los tags existentes con sus respectivos commit ID.

- **git push origin --tags**                                     -- Se utiliza para cargar los tags en el repositorio remoto, es decir GitHub; antes de enviarlos hay que realizar un pull para traer toda la                                                               información, siendo esta una buena práctica.

- **git tag -d nombre del tag**                                  -- Se utiliza para borrar un tag, vale la pena resaltar que este comando no borra el tag de GitHub, solo de git.

- **git push origin :refs/tags/nombre del tag**                  -- Una vez eliminado el tag desde git, con este comando se procede a eliminar el tag también en GitHub.

- **git show-branch**                                             -- Muestra de una manera más detallada las ramas y sus mas recientes commits.

- **git show-branch --all**                                       -- Sigue siendo información detallada, pero a su vez muestra también las ramas existentes en GitHub, es eficiente en caso de que                                                                desees saber si hay ramas sin cargar en el repositorio.

- **gitk**                                                 -- Interfaz gráfica para ver la distribución de ramas y commits, además del estado de los archivos acorde a cada commit.

- **git clone dirección del repositorio web**             -- Clona repositorios públicos en el disco duro/local, mas no es para ambientes colaborativos.

- **fork** -- en GitHub se utiliza para crear un proyecto igual al de otro usuario de git y contribuir, permite comparar el estado del proyecto clonado con el original y a su vez contribuir         mediante pull requests.

- **git remote add nombre de la variable link del repositorio**  -- Se utiliza para agregar más repositorios en git

- **pull request**  -- estado de revisión de código en GitHub antes de realizar un commit, se utiliza para asignar a terceros que revisen el código antes de combinar con la rama master.

- **git rebase**  -- *IMPORTANTE -- SIEMPRE SE HACE PRIMERO SOBRE LA RAMA QUE SE DESEA ELIMINAR Y LUEGO SOBRE LA QUE SE DESEA MANTENER, EN CASO DE NO HACERLO DE ESTA MANERA HAY QUE UTILIZAR GIT RESET. REBASE SE RECOMIENDA UTILIZARLO SOLO EN LOCAL, EN GIT ..*

- **git rebase rama a la que se desea unir sin dejar rastros de origen**   --- Siempre se debe de hacer desde la rama que se desea unificar, y                                                                          siempre se hace primero desde la rama que se desea eliminar.

- **git stash** -- *se utiliza para congelar temporalmente los cambios realizados en un proyecto para así poder moverse entre ramas o commits y ver las diferentes versiones sin afectar los cambios congelados en stash. a su vez, stash nos permite ya sea borrar esos cambios que ya fueron guardados en el código o incluso mover dichos cambios a una rama nueva sin afectar la rama en la que se estaba trabajando.*
Con este comando congelamos los cambios realizados en el código a stash, de forma que no es necesario realizar un commit. A su vez nos permite ver el código sin los                   cambios, tal cual estaba en el commit mas reciente

- **git stash list**    -- Vemos todos los stash existentes, identificados por el commit reciente al realizar el stash.

- **git stash pop**    -- Se utiliza para descongelar los cambios y verlos nuevamente en el código.   

- **git stash branch nombre de la rama**     --- Con este comando podemos mover los cambios a una nueva rama, de forma que podemos seguir trabajando en ellos en una nueva rama sin alterar la rama anterior. Todo esto es válido siempre y cuando no se haya realizado un commit aún.  

- **git stash drop**    -- Se utiliza para borrar los cambios congelados del stash, por ende desaparecen y el código regresa a su estado de commit mas reciente.     

- **git clean --dry-run**  -- Este comando analiza acerca de los archivos duplicados o innecesarios que podrían ser borrados.

- **git clean -f**         -- Se utiliza para eliminar los archivos sin seguimiento del repositorio en local. Entiéndase que los archivos sin seguimiento son los archivos que están dentro del directorio pero no en el repositorio en sí.
Este comando no aplica para carpetas, en caso de haber carpetas innecesarias las mismas deben de ser eliminadas manualmente, tampoco aplican las extensiones o rutas agregadas al .gitignore.

- **git log --oneline**    -- Se utiliza para ver en una sola línea el historial de commits del proyecto.

- **git cherry-pick id del commit**    -- Se utiliza para mover un commit al HEAD de la rama deseada, fusionando el commit anterior. Es una mala práctica ya que altera la historia de los commits. Se puede aplicar entre diferentes ramas, es decir, traer un commit de una rama secundaria a la rama principal por ejemplo. Nunca entre commits de una misma rama.

- **git commit --amend**  -- Este comando se utiliza para agregar a un commit existente cambios que no se agregaron por accidente una vez generado el commit. Es importante que una vez realizados los cambios "olvidados" se agreguen a staging mediante "git add .", y no se utilice el comando -am ya que eso sobreescribirá el commit que deseamos corregir. Una vez                        
agregados los cambios olvidados se escribe este comando y se procede a editar el mensaje del commit existente.

- **reset --soft y --hard**        -    *soft* regresa al commit seleccionado sin borrar la información que hubiese en staging momentos antes de realizar el commit al que nos estamos moviendo (visible con git status, una vez aplicado el reset soft). Por su parte *hard* regresa al commit deseado borrando todo, incluyendo lo agregado al staging.

- **git reflog**                -- Con este comando vemos la historia real de nuestro proyecto, incluyendo resets realizados, archivos borrados.. aciertos y errores. *EN GIT NADA SE BORRA*

- **git reset id del head deseado**   -- Este comando nos regresa al head que deseemos acorde a lo visualizado en reflog, no obstante mantiene los cambios realizados en tal momento en el staging.

- **git reset --hard id del commit deseado**  -- este comando nos regresa al commit deseado, no obstante borra todo lo que estuviese en el staging en dicho commit.

- **git grep**                               -- Se utiliza para encontrar palabras y etiquetas en el código.

- **git log**                                -- Se utiliza para encontrar palabras en el historial de los commits.

- **git grep -n palabra**                    -- Este comando arroja como resultado la ubicación y número de línea de la palabra que se esté buscando.

- **git grep -n "código o etiqueta"**        -- Este comando arroja como resultado la ubicación y número de línea del código que se esté buscando, se debe de escribir dentro de comillas.

- **git grep palabra**                    -- Este comando arroja como resultado la ubicación o nombre de archivo de la palabra que se esté buscando.

- **git grep "código o etiqueta"**        -- Este comando arroja como resultado la ubicación o no nombre del archivo del código que se esté buscando, se debe de escribir dentro de comillas.

- **git grep -c palabra**                    -- Este comando arroja como resultado la ubicación y el número de veces en la que aparece la palabra que se esté buscando.

- **git grep -c "código o etiqueta"**        -- Este comando arroja como resultado la ubicación y el número de veces en la que aparece el código que se esté buscando, se debe de escribir dentro                                           de comillas.

- **git log -S "nombre de la palabra que se esté buscando"**            -- Este comando se utiliza para buscar en el log de los commits, la S debe de ser en mayúscula y el criterio de búsqueda                                                                      debe de escribirse dentro de las comillas.

- **git shortlog**                        -- Con este comando se reflejan todos los commits sin tanto texto de por medio, de hecho solo se muestran los mensajes de cada commit realizado por cada                                        colaborador del proyecto.

- **git shortlog -sn**                    -- Resume en una lista todos los commits realizados por cada usuario, no se muestran los commits borrados.

- **git shortlog -sn --all**              -- Muestra todos los commits realizados, incluso los borrados a través de reset hard.

- **git shortlog -sn --all --no-merges**  --  Muestra todos los commits, incluso los borrados pero no los creados a través de merge.

- **git confif --global alias.nombre del alias "comando largo que se desea resumir en un alias"**    -- Este comando es para crear un alias a nivel global que se guardará en la configuración                                                                                                   global y por ende no se borrará al cerrar la línea de comandos. Dentro de las comillas no es                                                                                                   necesario escribir git nuevamente.  

- **git blame nombre del archivo**     -- Muestra línea por línea quienes son los responsables del código actual.

- **git blame -c nombre del archivo**  -- Muestra línea por línea quienes son los responsables del código actual, pero con en un formato indentado.

- **git comando --help**               -- Abre una pestaña en el navegador con toda la documentación del comando en interés, útil para aprender.

- **git blame archivo -Lnúmero de línea inicial,número de línea final**  -- Muestra línea por línea quienes son los responsables del código actual a través de las líneas seleccionadas en el                                                                       archivo deseado.

- **git blame archivo -Lnúmero de línea inicial,número de línea final -c**    -- Muestra línea por línea quienes son los responsables del código actual a través de las líneas seleccionadas en el                                                                             archivo deseado de una manera indentada.

- **git branch -r**                    -- Muestra las ramas cargadas en remoto, aparecen en color rojo.

- **git branch -a**                    -- Muestra todas las ramas creadas, en blanco aparecen las que están en local y en rojo las que están en remoto

- **git branch -d nombre de la rama**  -- Borra una rama.


