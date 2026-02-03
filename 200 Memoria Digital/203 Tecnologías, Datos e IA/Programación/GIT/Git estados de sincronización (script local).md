Los estados indican la relación entre tres capas de [[Git]]:

1. **Working tree**: archivos en la computadora local
    
2. **Repositorio local**: commits existentes en la rama actual
    
3. **Repositorio remoto**: repositorio de referencia configurado para la rama (upstream)
    

El repositorio remoto no es necesariamente origin; depende de cómo esté configurada la rama.

---

## [OK] — sincronizado y limpio

No existen cambios locales en archivos.  
No existen commits locales pendientes de subir.  
No existen commits remotos pendientes de bajar.

La rama local y su upstream están alineados.

---

## [LOCAL] — cambios locales, pero sincronizado

Existen cambios en el working tree:

- archivos modificados
    
- archivos nuevos
    
- archivos borrados
    

No existen commits locales ni remotos pendientes.

El trabajo aún no ha sido versionado.

---

## [AHEAD] — commits locales no subidos

Existen uno o más commits en el repositorio local que no están en el repositorio remoto configurado como upstream.

La rama local está adelantada respecto a su upstream.

Acción habitual: `git push`

---

## [BEHIND] — commits remotos no bajados

El repositorio remoto configurado como upstream contiene commits que no existen localmente.

La rama local está atrasada respecto a su upstream.

Acción habitual: `git pull`

---

## [DIVERGED] — conflicto potencial

La rama local y su upstream han avanzado de forma independiente.

Existen commits distintos en ambos lados.

Requiere intervención manual antes de continuar.

Acciones posibles:

- `git pull --rebase`
    
- resolución manual de conflictos
    
- revisión del historial
    

---

## Resumen

|Etiqueta|Estado|
|---|---|
|[OK]|Rama local alineada y sin cambios|
|[LOCAL]|Cambios locales sin commit|
|[AHEAD]|Commits locales no subidos|
|[BEHIND]|Commits remotos no bajados|
|[DIVERGED]|Conflicto potencial|

---

## Nota técnica

El script usa el upstream de la rama actual para determinar los estados de sincronización.  
Si una rama no tiene upstream configurado, el repositorio se omite.