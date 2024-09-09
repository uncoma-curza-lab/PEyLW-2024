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
   git checkout -gh-pages

### 5. Crear una nueva rama para tus cambios
   ```bash
   git checkout -b mi_nueva_rama
   ```
   Reemplazar "mi_nueva_rama" con un nombre descriptivo para tu nueva rama (por ejemplo, "nombre_usuario-laboratorio2").

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
   ```
   Estos comandos descargan los cambios más recientes del repositorio remoto y actualizan tu rama local `gh-pages` con ellos.

### 8. Fusionar tu rama con gh-pages
   ```bash
   git checkout gh-pages
   git pull
   git merge mi_nueva_rama
   ```
   Reemplaza `mi_nueva_rama` con el nombre de tu rama.

   * **Resolver conflictos:** Si hay conflictos, Git te indicará los archivos afectados. Editalos manualmente para resolver las diferencias y luego hacé commit de los cambios.

### 9. Subir los cambios al repositorio remoto
   ```bash
   git push origin gh-pages
   ```

### Resumen de los pasos:
1. **Clonar:** Descarga el repositorio completo. **UNA SOLA VEZ**, luego se deberá actualizar gh-pages como en el punto 6.
2. **Crear rama:** Crea una nueva rama para tus cambios.
3. **Realizar cambios:** Edita los archivos y guarda.
4. **Commitear:** Guarda los cambios en el historial local.
5. **Cambiar a gh-pages:** Prepararse para fusionar.
6. **Actualizar gh-pages:** Obtener los últimos cambios de la rama remota.
7. **Fusionar:** Combinar tu rama con gh-pages.
8. **Subir:** Publicar los cambios en el repositorio remoto.



