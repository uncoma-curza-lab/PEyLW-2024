# PEyLW-2024
Programación estatica y laboratorio web - 2024

---

## Uso: Ramas Git y Fusionando con `gh-pages`

### 1. Clonar el repositorio (se hace una sola vez)
* **Abrir terminal o línea de comandos.**
* **Navegar hasta la carpeta donde vas a guardar tu proyecto localmente.**
* **Ejecutar el siguiente comando:**
   ```bash
   git clone https://github.com/uncoma-curza-lab/PEyLW-2024.git
   ```
   Este comando descargará una copia completa del repositorio en tu computadora y creará una nueva carpeta llamada "PEyLW-2024".

### 2. Ingresar al directorio del proyecto
   ```bash
   cd PEyLW-2024
   ```

### 3. Verificar las ramas existentes
   ```bash
   git branch -a
   ```
   Esto mostrará todas las ramas locales y remotas.
   
### 4. Mover a rama gh-pages
   ```bash
   git checkout gh-pages
   ```
### 5. Crear una nueva rama para tus cambios
   ```bash
   git checkout -b <nombre_usuario>-<tarea_o_laboratorio>
   ```
   Reemplazar "<nombre_usuario>-<tarea_o_laboratorio>" con un nombre descriptivo para tu nueva rama (por ejemplo, "nombre_usuario-laboratorio2").

### 6. Realizar tus cambios
   * **Editar los archivos:** Usar tu editor de código (recomendamos VSCode) para los cambios necesarios en los archivos de tu proyecto.
   * **Guardar los cambios:** Guardar los archivos modificados.

### 7. Commitea tus cambios
   ```bash
   git add .  # Agrega todos los cambios al área de staging
   git commit -m "Nombre y Apellido - Labo #"
   git push --set-upstream origin nombre_branch
   ```
   Reemplaza "Nombre y Apellido - Labo #" con tu nombre y apellido y el número de laboratorio que entregas.

   Estos comandos descargan los cambios más recientes del repositorio remoto y actualizan tu rama local `gh-pages` con ellos.

### 8. Fusionar tu rama con gh-pages
   ```bash
   git checkout gh-pages
   git pull
   git merge <nombre_usuario>-<tarea_o_laboratorio>
   ```
   Reemplaza `mi_nueva_rama` con el nombre de tu rama.

   * **Resolver conflictos:** Si hay conflictos, Git te indicará los archivos afectados. Editalos manualmente para resolver las diferencias y luego hacé commit de los cambios.

### 9. Subir los cambios al repositorio remoto
   ```bash
   git push origin gh-pages
   ```

### 10. Tener en cuenta

Cada vez que se trabaje sobre una rama se deben realizar un git fetch all para actualizar las ramas.

   ```bash
   git fetch --all
   ```

### Resumen de los pasos:

1. [Clonar el repositorio]
2. [Entrar en el directorio del proyecto]
3. [Verificar las ramas disponibles]
4. [Cambiar a la rama `gh-pages`]
5. [Crear una nueva rama para tus cambios]
6. [Realizar cambios en los archivos]
7. [Agregar y hacer commit de los cambios]
8. [Fusionar tu rama con `gh-pages`]
9. [Subir los cambios fusionados al repositorio remoto]
10. [Actualizar ramas]

