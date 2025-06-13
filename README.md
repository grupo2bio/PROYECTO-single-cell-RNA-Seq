# PROYECTO-single-cell-RNA-Seq
![image](https://github.com/user-attachments/assets/096afa6e-1ce9-4a9a-9d27-31e5c165f553)

Este proyecto tiene como objetivo analizar datos transcriptómicos a nivel de célula individual para explorar la heterogeneidad celular en un tejido o condición experimental utilizando herramientas como **Seurat**, **Scanpy**, y visualización en UMAP/t-SNE.

## Objetivos

- Preprocesamiento y control de calidad de datos scRNA-Seq.
- Normalización y detección de genes variables.
- Análisis de reducción de dimensionalidad (PCA, UMAP, t-SNE).
- Clustering de células y anotación de tipos celulares.
- Identificación de genes marcadores por clúster.

## Estructura del proyecto
Nuestro proyecto contiene un branch principal "Main".
El comando git branch -a se utilizó para listar todas las ramas del repositorio, tanto locales como remotas. La salida muestra que la rama local activa es main (indicada con un asterisco), y que existe una rama remota llamada origin/main, la cual es también la rama principal del repositorio en GitHub. Además, se observa que remotes/origin/HEAD apunta a origin/main, lo que confirma que main es la rama por defecto del repositorio remoto. Esta información permite verificar en qué rama se está trabajando y cómo se relaciona con el repositorio en línea.

![image](https://github.com/user-attachments/assets/072c8e96-8197-4c46-a3ba-8fa221b5a2d8)

![image](https://github.com/user-attachments/assets/8db462a0-d420-48ce-a86e-d0b2aa638ce1)

Se crearon 
![image](https://github.com/user-attachments/assets/c95ab11c-9166-482e-a2ea-650c38ee93ad)

![image](https://github.com/user-attachments/assets/b660446b-c8a0-439f-8152-338ff6a9c265)

PROYECTO-single-cell-RNA-Seq/
Se crearon las carpetas `data/`, `scripts/`, `results/` y `docs/` para organizar de forma estructurada los contenidos del proyecto. La carpeta `data/` está destinada a almacenar archivos de datos brutos y preprocesados, como archivos `.h5`, `.mtx` o `.csv`. En `scripts/` se ubican los códigos en R o Python utilizados para el análisis, por ejemplo con herramientas como Seurat o Scanpy. La carpeta `results/` contiene los resultados generados, como gráficas, tablas o archivos serializados. Finalmente, `docs/` reúne documentación relevante, incluyendo manuales, referencias y guías relacionadas con el proyecto.

![image](https://github.com/user-attachments/assets/6015e67f-a15c-4d59-959d-4b17ae4bbe59)

Se utilizaron los comandos cd, ls y ls -l para navegar y visualizar el contenido del repositorio clonado en la máquina virtual. El comando cd PROYECTO-single-cell-RNA-Seq permitió ingresar al directorio del proyecto. Luego, ls mostró una lista básica de archivos y carpetas dentro de ese directorio. Finalmente, ls -l se utilizó para obtener una vista detallada de los archivos y carpetas, incluyendo sus permisos, propietarios, tamaño y fecha de modificación. La salida de este último comando permite verificar quién tiene acceso a los archivos y qué tipo de permisos tiene cada usuario (lectura, escritura y ejecución), lo que es útil para el manejo seguro y correcto del proyecto.

