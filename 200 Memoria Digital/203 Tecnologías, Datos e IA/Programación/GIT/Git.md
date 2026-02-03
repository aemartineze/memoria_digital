## ¿Qué es Git?
Git es un **sistema de control de versiones distribuido** que permite registrar, comparar y recuperar cambios en archivos a lo largo del tiempo.

Su objetivo principal es **mantener un historial confiable de cambios** y facilitar el trabajo individual o colaborativo sobre un mismo conjunto de archivos.

---

## ¿Qué problema resuelve?
Antes de Git, los cambios se gestionaban con:
- copias de archivos (`final_v1`, `final_v2`, `final_final`)
- pérdida de historial
- dificultad para volver atrás
- conflictos al trabajar con otras personas

Git resuelve esto al:
- guardar cada cambio como un **commit**
- permitir volver a cualquier estado anterior
- manejar versiones paralelas sin duplicar archivos

---
## Idea clave (modelo mental)

Git funciona como una **línea de tiempo de tu proyecto**.
Cada commit es una fotografía del estado de los archivos en un momento específico.  
No guarda solo el archivo final, sino **cómo fue cambiando**.

---
## Conceptos fundamentales

- **Repositorio**  
  Carpeta que contiene archivos y su historial de cambios.

- **Commit**  
  Registro de un cambio con un mensaje que explica qué se hizo y por qué.

- **Historial**  
  Secuencia ordenada de commits que muestra la evolución del proyecto.

- **Branch (rama)**  
  Línea de trabajo independiente que permite probar cambios sin afectar la principal.

- **Repositorio local**  
  Copia del proyecto que vive en tu computadora.

- **Repositorio remoto**  
  Copia del repositorio que vive en un servidor (por ejemplo, en [[GitHub]]).

- **Sincronización**  
  Proceso de enviar y recibir commits entre el repositorio local y el remoto.

---

## Qué NO es Git
- No es una plataforma web
- No es solo para programadores
- No reemplaza copias de seguridad, pero las mejora
- No requiere internet para funcionar localmente

---

## Relación con otras notas
- Para aprender **comandos y flujo mínimo** → [[Git básico]]
- Para entender la **plataforma donde se alojan repos** → [[GitHub]]

---

## Cuándo conviene usar Git
- Proyectos que evolucionan con el tiempo
- Notas importantes (por ejemplo, bóvedas de Obsidian)
- Scripts, documentos, código, investigaciones
- Cualquier cosa que quieras **entender cómo cambió**

