# PROYECTO-single-cell-RNA-Seq
![image](https://github.com/user-attachments/assets/096afa6e-1ce9-4a9a-9d27-31e5c165f553)

Este proyecto tiene como objetivo analizar datos transcriptómicos a nivel de célula individual para explorar la heterogeneidad celular en un tejido o condición experimental utilizando herramientas como **Seurat**, **Scanpy**, y visualización en UMAP/t-SNE.

## Objetivos

- Preprocesamiento y control de calidad de datos scRNA-Seq.
- Normalización y detección de genes variables.
- Análisis de reducción de dimensionalidad (PCA, UMAP, t-SNE).
- Clustering de células y anotación de tipos celulares.
- Identificación de genes marcadores por clúster.


## Creación del repositorio en GitHub
Se accedió a GitHub, se creó una cuenta y posteriormente un nuevo repositorio con el nombre PROYECTO-single-cell-RNA-Seq. Se añadió una descripción clara del propósito del proyecto y se seleccionó la licencia MIT, que permite su reutilización y modificación.

![image](https://github.com/user-attachments/assets/d256967c-aa21-4803-a661-c3955cf2dc1c)


### Colaboración en grupo y gestión de acceso
Para facilitar el trabajo colaborativo, se compartió el acceso al repositorio de GitHub con todos los miembros del grupo siguiendo estos pasos:

1. Se accedió al repositorio desde la cuenta que lo creó.
2. En la parte superior derecha del repositorio, se hizo clic en **Settings**.
3. En el menú lateral, se seleccionó **Collaborators**.
4. Se ingresaron los nombres de usuario de GitHub de los integrantes en el campo de búsqueda.
5. Se hizo clic en **Add** junto a cada usuario para enviar la invitación como colaboradores.
6. Cada miembro aceptó la invitación desde su cuenta.

## Estructura del proyecto
Nuestro proyecto contiene un branch principal "Main".
El comando git branch -a se utilizó para listar todas las ramas del repositorio, tanto locales como remotas. La salida muestra que la rama local activa es main (indicada con un asterisco), y que existe una rama remota llamada origin/main, la cual es también la rama principal del repositorio en GitHub. Además, se observa que remotes/origin/HEAD apunta a origin/main, lo que confirma que main es la rama por defecto del repositorio remoto. Esta información permite verificar en qué rama se está trabajando y cómo se relaciona con el repositorio en línea.

![image](https://github.com/user-attachments/assets/072c8e96-8197-4c46-a3ba-8fa221b5a2d8)

### Verificacion de Git 
Antes de comenzar a trabajar con el proyecto, se verificó que Git estuviera instalado en el sistema Ubuntu. Para ello, se abrió una terminal y se ejecutó el comando git --version. Si Git estaba instalado, el sistema mostraba la versión correspondiente. En caso de que no lo estuviera, se procedía a instalarlo utilizando el comando sudo apt install git.

![image](https://github.com/user-attachments/assets/ac00bb0c-d033-4102-88aa-b5e63bfeddef)

### Clonación del repositorio
Una vez verificada la disponibilidad de Git, se clonó el repositorio del proyecto desde GitHub. Este proceso se realizó ejecutando el comando git clone https://github.com/tuusuario/PROYECTO-single-cell-RNA-Seq.git, lo que descargó una copia local del proyecto en una carpeta llamada PROYECTO-single-cell-RNA-Seq. Luego, se accedió al directorio del proyecto con el comando cd PROYECTO-single-cell-RNA-Seq para iniciar el trabajo.

![image](https://github.com/user-attachments/assets/5557c810-e5c1-4a49-8084-98d116ad586a)

### Creación de carpetas
Para organizar el proyecto, se crearon las carpetas data/, scripts/, results/ y docs/. Esto se realizó con el comando mkdir desde la terminal. El objetivo de utilizar estos comandos es organizar adecuadamente los archivos del análisis, separando los datos, los scripts, los resultados generados y la documentación, lo cual facilita el trabajo colaborativo, el mantenimiento del proyecto y la reproducibilidad de los análisis.

![image](https://github.com/user-attachments/assets/c95ab11c-9166-482e-a2ea-650c38ee93ad)

### Guardando cambios en Git
Luego de crear las carpetas `data/`, `scripts/`, `results/` y `docs/` para estructurar el proyecto, se intentó guardar estos cambios en el repositorio utilizando Git. Para ello, se ejecutaron los comandos necesarios para registrar y subir los cambios al repositorio remoto en GitHub. Primero, se agregaron las carpetas con `git add .`, luego se creó un mensaje de confirmación con `git commit -m "Creación de carpetas del proyecto"`, y finalmente se intentó subir los cambios con `git push origin main`. Sin embargo, como el repositorio remoto ya tenía cambios que no estaban en la copia local, Git rechazó el push. Para solucionarlo, se utilizó `git pull --rebase origin main` para integrar los cambios remotos con los locales, y después se repitió `git push origin main` con éxito, logrando guardar correctamente la estructura del proyecto en el repositorio compartido.

![image](https://github.com/user-attachments/assets/8db462a0-d420-48ce-a86e-d0b2aa638ce1)

### Descripción de las carpetas
Se crearon las carpetas `data/`, `scripts/`, `results/` y `docs/` para organizar de forma estructurada los contenidos del proyecto. La carpeta `data/` está destinada a almacenar archivos de datos brutos y preprocesados, como archivos `.h5`, `.mtx` o `.csv`. En `scripts/` se ubican los códigos en R o Python utilizados para el análisis, por ejemplo con herramientas como Seurat o Scanpy. La carpeta `results/` contiene los resultados generados, como gráficas, tablas o archivos serializados. Finalmente, `docs/` reúne documentación relevante, incluyendo manuales, referencias y guías relacionadas con el proyecto.

![image](https://github.com/user-attachments/assets/b660446b-c8a0-439f-8152-338ff6a9c265)

### Navegación y visualización de archivos
Se utilizaron los comandos cd, ls y ls -l para navegar y visualizar el contenido del repositorio clonado en la máquina virtual. El comando cd PROYECTO-single-cell-RNA-Seq permitió ingresar al directorio del proyecto. Luego, ls mostró una lista básica de archivos y carpetas dentro de ese directorio. Finalmente, ls -l se utilizó para obtener una vista detallada de los archivos y carpetas, incluyendo sus permisos, propietarios, tamaño y fecha de modificación. La salida de este último comando permite verificar quién tiene acceso a los archivos y qué tipo de permisos tiene cada usuario (lectura, escritura y ejecución), lo que es útil para el manejo seguro y correcto del proyecto.

![image](https://github.com/user-attachments/assets/6015e67f-a15c-4d59-959d-4b17ae4bbe59)

## Creación del archivo .gitignore
## 📄 Creación del archivo `.gitignore`

Para evitar que archivos innecesarios, temporales o específicos del sistema operativo se suban al repositorio, se creó un archivo llamado `.gitignore` en el directorio raíz del proyecto. 

Primero, se generó el archivo vacío utilizando el comando:

```bash
touch .gitignore
Luego se abrió con un editor de texto mediante:

bash
Copiar
Editar
nano .gitignore
Dentro del archivo, se agregaron reglas específicas para excluir ciertos tipos de archivos y carpetas del control de versiones. Por ejemplo:

gitignore
Copiar
Editar
# Archivos del sistema
.DS_Store
Thumbs.db

# Archivos de Python
__pycache__/
*.pyc
*.pyo

# Archivos de R
.Rhistory
.RData
.Rproj.user/

# Configuraciones locales
.vscode/
.idea/

# Resultados y archivos temporales
results/
*.log
*.tmp
Después de guardar los cambios (Ctrl + O, Enter, y salir con Ctrl + X), se verificó el contenido del archivo con:

bash
Copiar
Editar
cat .gitignore
A continuación, se agregaron los cambios al área de preparación de Git:

bash
Copiar
Editar
git add .gitignore
Se registró el cambio con un mensaje descriptivo:

bash
Copiar
Editar
git commit -m "Agregar archivo .gitignore con reglas para Ubuntu, Python, R y archivos temporales"
Y finalmente, se subieron los cambios al repositorio remoto con:

bash
Copiar
Editar
git push origin main
Gracias a este archivo .gitignore, el repositorio se mantiene más limpio y organizado, incluyendo únicamente los archivos necesarios para el análisis, lo que facilita el trabajo colaborativo y evita subir archivos sensibles o irrelevantes.

arduino
Copiar
Editar

¿Deseas que prepare las otras secciones también en este estilo?



d



Para evitar que archivos innecesarios, temporales o específicos del sistema operativo se suban al repositorio, se creó un archivo llamado .gitignore en el directorio raíz del proyecto. Primero, se generó el archivo vacío utilizando el comando touch .gitignore, y luego se abrió con un editor de texto mediante nano .gitignore, aunque también se puede usar cualquier otro editor como vim o code.

Dentro del archivo .gitignore, se agregaron reglas específicas para excluir ciertos tipos de archivos y carpetas del control de versiones. 

Después de guardar los cambios en el archivo con las combinaciones de teclas (Ctrl + O, Enter y Ctrl + X para salir en nano), se verificó su contenido con el comando cat .gitignore para asegurarse de que las reglas se habían guardado correctamente. A continuación, se agregó el archivo al área de preparación de Git con git add .gitignore, y luego se registró el cambio con un mensaje descriptivo usando git commit -m "Agregar archivo .gitignore con reglas para Ubuntu, Python, R y archivos temporales".

Finalmente, se subieron los cambios al repositorio remoto ejecutando el comando git push origin main. Gracias a este archivo .gitignore, el repositorio se mantiene más limpio y organizado, incluyendo únicamente los archivos necesarios para el análisis, lo que facilita el trabajo colaborativo y evita subir archivos sensibles o irrelevantes.

![image](https://github.com/user-attachments/assets/115489c8-97b3-4015-9225-b3304f210868)

El archivo .gitignore indica a Git qué archivos o carpetas deben ser ignorados y no subidos al repositorio remoto. Esto es útil para evitar que archivos temporales, de configuración local, datos grandes o generados automáticamente, y archivos específicos del sistema operativo se mezclen con el código fuente. Por ejemplo, se ignoraron archivos de sistema como .DS_Store y Thumbs.db, carpetas generadas automáticamente por Python como __pycache__/ o archivos .pyc, archivos temporales y de historial de R como .Rhistory o .RData, así como carpetas de configuración local como .vscode/ o .idea/. También se excluyeron carpetas como results/ y archivos .log o .tmp, que se generan durante el análisis y no necesitan ser compartidos. Así, el repositorio se mantiene limpio y ligero, facilitando el trabajo colaborativo y evitando subir información innecesaria o sensible.

![image](https://github.com/user-attachments/assets/c9bf58de-e728-41f9-9d28-6da1297a4c28)

El comando cat .gitignore se utiliza para mostrar en la terminal el contenido completo del archivo .gitignore. Esto permite revisar rápidamente qué reglas y patrones se han definido para que Git ignore ciertos archivos o carpetas dentro del proyecto. Es una forma sencilla y directa de verificar que el archivo .gitignore contiene las exclusiones correctas sin necesidad de abrir un editor de texto.

