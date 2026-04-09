# Catastro Minero de Salta — Análisis en QGIS

## Descripción

Proyecto de análisis geoespacial sobre el catastro minero oficial de la provincia de Salta, Argentina. Complementa el análisis de datos realizado en Python/Jupyter ([ver repositorio](https://github.com/Camilamop/catastro-minero-salta-mining-registry-salta)).

El dataset proviene del Geoportal oficial de la provincia y contiene 4.104 registros de concesiones mineras con geometría MULTIPOLYGON, datos de titulares, minerales, estados legales y fechas de inicio.

## Pregunta de investigación

¿Cómo se distribuye espacialmente la actividad minera en Salta y qué patrones territoriales emergen en relación con otros usos del suelo, cuencas hídricas y comunidades indígenas?

## Estructura del repositorio

```
catastro-minero-salta-qgis/
├── datos/
│   ├── raw/          # Dataset original sin modificar (fuente oficial)
│   └── procesado/    # Capas derivadas y tablas unidas
├── mapas/            # Exportaciones cartográficas (.png, .pdf)
├── informe/          # Documentos de resultados
└── catastro_minero_salta.qgz   # Proyecto QGIS
```

## Requisitos

- **QGIS 3.34.x (LTR)** — Versión utilizada para este proyecto
- Sistema de referencia de coordenadas: WGS84 / EPSG:4326
- Plugins recomendados: QuickMapServices (para basemaps)

## Fuente de datos

- **Organismo:** Secretaría de Minería de la Provincia de Salta
- **URL:** https://geoportal.salta.gob.ar/catalogue/uuid/72c41757-bdee-4215-ab4e-9a02fc56954e
- **Formato:** Shapefile (MULTIPOLYGON, WGS84)
- **Registros:** 4.104 concesiones mineras
- **Última actualización del dataset:** Diciembre 2025

> Los datos no están incluidos en este repositorio por su tamaño. Descargalos desde la URL oficial y colocalos en `datos/raw/`.

## Contenido cartográfico

| Mapa | Descripción |
|------|-------------|
| Distribución general | Extensión y densidad de concesiones en la provincia |
| Por mineral | Clasificación según el recurso declarado |
| Por titular | Concentración de concesiones por actor |
| Por estado legal | Vigentes, caducas, en trámite |

## Consideraciones éticas

El dataset es de carácter público oficial. El análisis incluye datos de personas físicas que, si bien son públicos en su rol de concesionarios mineros registrados, son tratados con las consideraciones éticas propias de la investigación en derechos humanos.

## Repositorio complementario

El análisis estadístico, modelado relacional y análisis de redes de este mismo dataset se encuentra en:
👉 [catastro-minero-salta-mining-registry-salta](https://github.com/Camilamop/catastro-minero-salta-mining-registry-salta)

## Autora

**Camila Agustina Mopty**  
Arquitecta | Becaria doctoral CONICET | Diplomatura en Ciencia de Datos (UTN)  
[LinkedIn](http://www.linkedin.com/in/camila-mopty) · camilamopty@gmail.com
