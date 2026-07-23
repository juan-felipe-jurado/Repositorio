# INSTRUCCIONES PARA CREAR

## Commit
### Commit desde la web de GitHub
1. Hacer el cambio (editar archivo, subir imagen, crear archivo nuevo, etc.).
2. Bajas hasta el final de la página, donde aparece la sección "Commit changes".
3. Ahí completas:
   - Título del commit: describe brevemente el cambio
   - Descripción: detalles adicionales si quieres
5. Click en "Commit changes" (botón verde).

### Commit desde tu computador con Git
1. Abre CMD: Busca **cmd** en el menú de inicio y ábrelo.
2. Ve a la carpeta donde quieres el repositorio:
  - **cd Desktop**
3. Si aún no tienes el repositorio clonado:
  - **git clone https://github.com/juan-felipe-jurado/Repositorio.git**
  - **cd Repositorio**
4. Si ya lo tienes clonado, solo entra a la carpeta
  - **cd Repositorio**
5. Cambia a la rama develop
  - **git checkout develop**
6. Configura tu identidad (solo la primera vez que usas Git)
  - **git config --global user.name "Tu Nombre"**
  - **git config --global user.email "tu-correo@ejemplo.com"**
7. Haz tus cambios: Edita o crea archivos normalmente (con el Bloc de notas, VS Code, etc.) dentro de esa carpeta.
8. Verifica qué cambió
  - **git status**
9. Agrega los archivos al commit
  - **git add instruction.md**
  - o para agregar todo: **git add .**
10. Haz el commit
  - **git commit -m "Agregar instruction.md"**
11. Sube los cambios a GitHub
 - **git push origin develop**
 - Si es la primera vez que subes esa rama, puede pedirte: **git push --set-upstream origin develop**

## Commit desde tu computador más simple
### Comando básico
- **git push origin nombre-de-tu-rama**
- Por ejemplo, si estás en develop: **git push origin develop**
### Primera vez que subes esa rama
Si la rama es nueva y no existe aún en GitHub, usa:
- **git push --set-upstream origin develop**
- o su forma corta: **git push -u origin develop**
Esto vincula tu rama local con la remota, para que después solo necesites escribir git push a secas.
### Después de la primera vez
Una vez vinculada la rama, para futuros cambios solo necesitas:
- **git push**
  
### Flujo completo típico
- **git add .**
- **git commit -m "Descripción del cambio"**
- **git push**
