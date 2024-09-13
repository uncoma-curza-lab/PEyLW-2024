Guía básica sobre cómo utilizar Git, cubriendo los pasos desde clonar un repositorio hasta subir cambios y trabajar con ramas.

### **1. Clonar un repositorio**
Para clonar un repositorio, necesitas la URL del mismo. Este comando creará una copia local del repositorio en tu máquina.

```bash
git clone <URL-del-repositorio>
```
Ejemplo:
```bash
git clone https://github.com/usuario/repo.git
```

### **2. Actualizar el repositorio local (Hacer pull)**
Para asegurarte de que tu repositorio local está actualizado con los últimos cambios del repositorio remoto, debes hacer un pull:

```bash
git pull
```

### **3. Crear y cambiar de rama**
Crear una nueva rama es útil para trabajar en una nueva característica o un bug sin afectar la rama principal. Para crear una nueva rama y cambiarte a ella:

```bash
git checkout -b <nombre-de-la-rama>
```
Ejemplo:
```bash
git checkout -b feature/nueva-funcionalidad
```

Para cambiar a una rama existente:
```bash
git checkout <nombre-de-la-rama>
```

### **4. Hacer cambios y agregar al staging**
Después de realizar cambios en los archivos, necesitas agregarlos al área de staging antes de hacer un commit.

Para agregar archivos específicos:
```bash
git add <ruta-del-archivo>
```
Para agregar todos los archivos modificados:
```bash
git add .
```

### **5. Hacer commit de los cambios**
Una vez que los archivos están en el área de staging, puedes hacer un commit. Esto guarda los cambios en tu repositorio local.

```bash
git commit -m "Mensaje descriptivo sobre los cambios"
```

### **6. Subir los cambios al repositorio remoto**
Para subir tus cambios locales a la rama en el repositorio remoto:

```bash
git push
```

### **7. Ver el estado del repositorio**
Para ver qué archivos han cambiado, cuáles están en el área de staging, y el estado general de tu repositorio:

```bash
git status
```

### **8. Ver el historial de commits**
Para ver el historial de commits en tu rama actual:

```bash
git log
```
