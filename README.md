# GitListaComando
> Lista de Comandos Memorias

## **Crear carpeta**  
mkdir escenario1

## **Listar Archivos**  
ls -la

**Iniciar registro en Git**  
git init

**Crear Archivo**  
echo "# primera linea de un fichero readme.md" > readme.md  
nano .gitignore (para no considerar en los commits)  
.*tmp

**Verificar Status de Cambios**  
git status

**Comitear cambios**  
git commit -m "commit de readme.md"

**Incluir cambios para enviar al commit**  
git add .

**Ver diferencia de versiones**  
git diff

**Descargar Interfaz para la difrencias**  
http://www.posoft.de/html/tkdiffMain.html  
Colocar en ruta C:\Program Files\Git\usr\bin

**Pasos para descargar al git  bash**  
_Conectar desde Github de forma remota_  
git remote add origin https://github.com/designmodo/html-website-templates

**Obtener las ramas o version que tiene las fuentes**  
git fetch origin

**Descargar en carpeta local git las fuentes de la rama seleccionada**  
git pull origin master

**Copiar desde Github Modo 2**  
git clone https://github.com/StartBootstrap/startbootstrap-freelancer .  
_(el . Indica que se copiara el contenido de la carpeta raiz en nuestra carpeta destino)_

**Subir al github**  
git push origin main

**Restaurar Archivos Eliminados**  
git checkout HEAD -- .

**Restaurar Cambios del Stage**  
git reset head readme.md

**Restaurar cambios del working y del staging**  
git reset --hard HEAD~1 

**Revertir cambio**  
git revert aa77752

**Generar una rama a partir de la Rama Master**  
git branch new_main master

**Posicionar sobre la rama new_main**  
git checkout new_main

**Listado de Ramas**  
git branch

**Listado de Ramas incluyendo Remotas**  
git branch -a

**Listado de Ramas incluyendo Remotas  con ultimo Commit**  
git branch -a -v

**Merge entre Ramas**  
git merge new_main master

**Eliminar Ramas**  
git branch -d new_main

**Crear nueva Rama y posicionarse en la nueva**  
git checkout -b new_rama main

**Identificar Usuario Cambio**  
git blame src/output.rs

**Tag para los cambios _(agrupa los cambios realizados luego del commit agregar tag)_**  
git tag -a v1.5 -m "version tag version 1.5"

**Guardar ultimo Commit luego de haber cambiado y tenerlo en staging(git add .)**  
git stash (Se ejecuta luego que tengamos algun cambio en el staging)

**Recuperar el ultimo commit guarda con stash**  
git stash apply

