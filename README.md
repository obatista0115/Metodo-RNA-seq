# Metodologías de Análisis Bioinformático (RNA-seq) 🧬

Este repositorio centraliza los flujos de trabajo bioinformáticos desarrollados durante mi formación en la materia de Secuenciación y Ciencias -Ómicas del **Máster en Bioinformática de la Universidad Internacional de La Rioja (UNIR) - 2025**. El objetivo es documentar y compartir pipelines estandarizados para el estudio del transcriptoma, desde el procesamiento de lecturas crudas hasta la interpretación biológica avanzada.

---

## 📂 Proyectos Disponibles

### 1. [Análisis de Obesidad (RNA-seq Bulk)](./Obesidad)
Estudio comparativo para identificar genes diferencialmente expresados (DEG) y caracterizar la variabilidad molecular entre distintos fenotipos de obesidad.

* **Estado:** Finalizado ✅
* **Workflow Técnico:** * **Control de Calidad:** `FastQC`.
    * **Cuantificación:** Seudoalineamiento con `Salmon` e importación con `tximport`.
    * **Análisis Estadístico:** Normalización y expresión diferencial con `DESeq2`.
    * **Análisis de Redes:** Construcción de redes de coexpresión con `igraph`.
    * **Enriquecimiento Funcional:** Análisis de rutas GO y KEGG con `gprofiler2`.
* **Visualización Científica:** Generación de Volcano plots y MA-plots con `ggplot2`, y mapas de calor (Heatmaps) con `pheatmap`.

---

### 2. [Single-cell RNA-seq (scRNA-seq)](./Single-cell)
Pipeline enfocado en el análisis de secuenciación de célula única para la caracterización de la heterogeneidad celular y descubrimiento de nuevos subtipos celulares.

* **Estado:** En desarrollo 🚧
* **Enfoque:** Procesamiento de matrices de conteo, control de calidad celular, reducción de dimensionalidad y clustering.

---

## 🛠️ Entorno de Trabajo
Los análisis están implementados principalmente en **R (v4.0+)**, utilizando librerías especializadas del ecosistema **Bioconductor**. Cada carpeta contiene la documentación específica para reproducir los resultados, incluyendo scripts en formato R Markdown (`.Rmd`).

---

## 👤 Autor
**Oriana Batista Ceballos** *Máster en Bioinformática - UNIR (2025)* 

---
*Este repositorio ha sido creado con fines académicos y de investigación. Para consultas sobre la implementación o los datos, por favor abre un 'Issue' en este repositorio.*
