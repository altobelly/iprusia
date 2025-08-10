# 🚀 Cómo subir tu lista M3U a GitHub

Esta guía te enseñará paso a paso cómo subir tu proyecto de lista M3U a GitHub para que otras personas puedan usarla.

## 📋 Prerequisitos

- Tener una cuenta en [GitHub](https://github.com)
- Tener Git instalado en tu computadora ([Descargar Git](https://git-scm.com/downloads))

## 🎯 Opción 1: Usando la interfaz web de GitHub (Más fácil)

### Paso 1: Crear un nuevo repositorio
1. Ve a [GitHub](https://github.com) e inicia sesión
2. Haz clic en el botón **"New"** o **"+"** → **"New repository"**
3. Completa los datos:
   - **Repository name**: `lista-canales-m3u` (o el nombre que prefieras)
   - **Description**: `Lista M3U de canales de televisión en español`
   - ✅ Marca **"Public"** (para que sea accesible públicamente)
   - ✅ Marca **"Add a README file"** (GitHub creará uno básico)
   - **Add .gitignore**: Selecciona "None" (ya tenemos nuestro .gitignore)
   - **Choose a license**: MIT License (recomendado)
4. Haz clic en **"Create repository"**

### Paso 2: Subir los archivos
1. En tu nuevo repositorio, haz clic en **"uploading an existing file"** o **"Add file"** → **"Upload files"**
2. Arrastra o selecciona estos archivos:
   - `canales.m3u`
   - `README.md` (reemplaza el que GitHub creó)
   - `.gitignore`
3. En la parte inferior:
   - **Commit title**: `Añadir lista M3U inicial con 25+ canales`
   - **Description**: `Lista completa de canales españoles, autonómicos e internacionales`
4. Haz clic en **"Commit changes"**

### Paso 3: Obtener la URL de tu lista
Tu lista estará disponible en:
```
https://raw.githubusercontent.com/TU_USUARIO/lista-canales-m3u/main/canales.m3u
```
*(Sustituye TU_USUARIO por tu nombre de usuario de GitHub)*

## 🖥️ Opción 2: Usando Git desde la línea de comandos

### Paso 1: Configurar Git (solo la primera vez)
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@example.com"
```

### Paso 2: Crear repositorio en GitHub
1. Sigue los pasos 1-4 de la Opción 1, pero **NO marques** "Add a README file"

### Paso 3: Inicializar repositorio local
```bash
# Navegar a tu carpeta del proyecto
cd C:\Users\ekate\Desktop\Canales

# Inicializar repositorio Git
git init

# Añadir todos los archivos
git add .

# Hacer el primer commit
git commit -m "Añadir lista M3U inicial con 25+ canales"

# Conectar con GitHub (sustituye TU_USUARIO)
git remote add origin https://github.com/TU_USUARIO/lista-canales-m3u.git

# Subir archivos a GitHub
git branch -M main
git push -u origin main
```

## 🔄 Cómo actualizar tu lista M3U

### Usando la interfaz web:
1. Ve a tu repositorio en GitHub
2. Haz clic en el archivo `canales.m3u`
3. Haz clic en el ícono del lápiz (✏️) para editar
4. Haz tus cambios
5. Scroll hacia abajo, añade un mensaje de commit
6. Haz clic en **"Commit changes"**

### Usando Git:
```bash
# Editar el archivo canales.m3u localmente
# Luego ejecutar:

git add canales.m3u
git commit -m "Actualizar canales - agregar [nombre del canal]"
git push
```

## 📱 Compartir tu lista M3U

Una vez subida, puedes compartir tu lista usando:

### URL directa del archivo:
```
https://raw.githubusercontent.com/TU_USUARIO/TU_REPOSITORIO/main/canales.m3u
```

### URL del repositorio:
```
https://github.com/TU_USUARIO/TU_REPOSITORIO
```

## 🎨 Personalizar tu repositorio

### Añadir badges al README:
```markdown
![GitHub last commit](https://img.shields.io/github/last-commit/TU_USUARIO/TU_REPOSITORIO)
![GitHub stars](https://img.shields.io/github/stars/TU_USUARIO/TU_REPOSITORIO)
![GitHub forks](https://img.shields.io/github/forks/TU_USUARIO/TU_REPOSITORIO)
```

### Crear releases:
1. Ve a tu repositorio → **"Releases"** → **"Create a new release"**
2. Tag: `v1.0.0`
3. Title: `Lista M3U v1.0 - Lanzamiento inicial`
4. Describe los canales incluidos
5. Adjunta el archivo `canales.m3u`
6. Haz clic en **"Publish release"**

## 🛡️ Consejos de seguridad

1. **Nunca subas**:
   - Contraseñas o tokens
   - Información personal
   - URLs privadas o con autenticación

2. **Revisa los enlaces**:
   - Asegúrate de que los streams son públicos
   - Verifica que tienes permiso para compartirlos

3. **Mantén actualizado**:
   - Revisa regularmente que los enlaces funcionen
   - Actualiza canales que cambien de URL

## 🆘 Solución de problemas

### Error: "Permission denied"
```bash
# Usar token de acceso personal en lugar de contraseña
# O configurar SSH keys
```

### Error: "Repository not found"
- Verifica que el nombre del repositorio sea correcto
- Asegúrate de que el repositorio existe en GitHub

### Los archivos no se ven
- Espera unos minutos, GitHub puede tardar en procesar
- Verifica que hiciste `git push` correctamente

## 📞 Contacto y soporte

Si tienes problemas:
1. Revisa la [documentación de GitHub](https://docs.github.com)
2. Busca en [GitHub Community](https://github.community)
3. Crea un issue en este repositorio

---

🎉 **¡Felicitaciones! Tu lista M3U ya está en GitHub y lista para compartir con el mundo.** 