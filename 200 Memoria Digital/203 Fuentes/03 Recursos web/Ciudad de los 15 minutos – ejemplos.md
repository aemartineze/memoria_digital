
Repositorios inspiración para un proyecto de [[Análisis de datos|análisis de datos]] para [[Quito]] bajo el concepto de [[Ciudad de 15 minutos|ciudad de 15 minutos]]
## 1. green-15min-city

**Repositorio:** https://github.com/GIScience/green-15min-city  
**Enfoque:** Modelo de accesibilidad urbana basado en tiempo de caminata.  
**Tecnologías:** [[Python]], análisis geoespacial, OpenStreetMap.  
**Qué hace:**
- Calcula áreas accesibles en 15 minutos.
- Usa red real de calles (no distancia en línea recta).
- Permite evaluar cobertura de servicios urbanos.

**Aplicación potencial:** Construcción de isocronas peatonales y medición de cobertura por barrio.

---

## 2. city_walkability

**Repositorio:** https://github.com/henryspatialanalysis/city_walkability  
**Enfoque:** Análisis de caminabilidad y acceso a equipamientos.  
**Tecnologías:** Python, GIS, análisis de redes.  
**Qué hace:**
- Calcula tiempos de viaje caminando.
- Genera mapas de accesibilidad.
- Evalúa proximidad a servicios.

**Aplicación potencial:** Medir porcentaje de población con acceso cercano a servicios básicos.

---

## 3. 15min-cities-Model

**Repositorio:** https://github.com/mohammadvhb/15min-cities-Model  
**Enfoque:** Modelo multimodal de accesibilidad urbana.  
**Tecnologías:** Python, visualización WebGIS.  
**Qué hace:**
- Simula acceso en distintos modos (caminar, bicicleta, automóvil).
- Permite comparar umbrales de 10, 15 y 30 minutos.
- Visualiza resultados en mapa interactivo.

**Aplicación potencial:** Evaluación de modelo ampliado incluyendo transporte público.

---

## 4. 15minute (OSM script)

**Repositorio:** https://github.com/Zverik/15minute  
**Enfoque:** Script ligero para análisis básico con OpenStreetMap.  
**Tecnologías:** OpenStreetMap, análisis de red.  
**Qué hace:**
- Calcula métricas simples de proximidad.
- Genera visualizaciones rápidas.

**Aplicación potencial:** Proyectos didácticos o pruebas exploratorias.

---

## Nota metodológica general

Estos repositorios comparten elementos técnicos comunes:

- Uso de red vial real modelada como grafo.
- Cálculo basado en tiempo de viaje, no solo distancia.
- Integración de datos de OpenStreetMap.

Para aplicar el enfoque a Quito se requeriría:

1. Descargar la red vial desde OpenStreetMap.
2. Definir categorías de servicios (salud, educación, comercio, ocio).
3. Calcular isocronas de 15 minutos.
4. Medir cobertura poblacional por barrio o zona censal.