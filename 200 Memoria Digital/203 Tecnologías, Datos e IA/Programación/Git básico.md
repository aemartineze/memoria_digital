## Crear un repositorio y sincronizarlo en local

### 1. Crear el repositorio remoto
- Crear un repositorio vacío en [[GitHub]] o GitLab.
- No agregar README, `.gitignore` ni licencia.

### 2. Inicializar Git en la carpeta local

~~~bash
cd ruta/de/la/carpeta
git init
~~~

### 3. Conectar la carpeta local con el repositorio remoto

~~~bash
git remote add origin URL_DEL_REPOSITORIO
~~~

El url del repositorio tiene .git

Verificar conexión:

~~~bash
git remote -v
~~~

### 4. Primer commit y primer push

~~~bash
git add .
git commit -m "Primer commit"
git branch -M main
git push -u origin main
~~~

La carpeta local queda sincronizada con el repositorio remoto.

## 5. Flujo básico de trabajo

### Subir cambios (push)

~~~bash
git add .
git commit -m "Mensaje del cambio"
git push
~~~

### Traer cambios (pull)

~~~bash
git pull
~~~


## 6. Clonar un repositorio

Permite descargar un proyecto desde GitHub a tu computadora.

### Comando básico

~~~bash
git clone URL_DEL_REPOSITORIO
~~~
---

## Reglas rápidas

- No hacer `git pull` con cambios sin commitear.
- Commits pequeños y claros.
- `push` envía cambios al remoto.
- `pull` trae cambios del remoto.

---

## Uso típico
Trabajo local → `git add` → `git commit` → `git push`  
Trabajo desde otro equipo → `git pull`
