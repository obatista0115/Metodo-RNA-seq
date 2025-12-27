# Análisis de Expresión Diferencial y Redes de Coexpresión en Obesidad (RNA-seq)

Este apartado contiene el flujo de trabajo bioinformático desarrollado para identificar genes diferencialmente expresados (**DEG**) y caracterizar la variabilidad molecular entre dos fenotipos de obesidad (Obeso 1 vs. Obeso 2).

El **RNA-seq** permite analizar el transcriptoma completo para entender la expresión génica y su asociación con mecanismos patológicos. En este proyecto, se aplicó un pipeline integral desde la cuantificación de transcritos hasta el enriquecimiento funcional.

> **Proyecto realizado para el Máster en Bioinformática, UNIR (2025).**

## 🧬 Flujo de Trabajo (Workflow)

1. **Control de Calidad:** Evaluación de lecturas crudas con `FastQC`.
2. **Cuantificación:** Seudoalineamiento y estimación de abundancias con `Salmon`.
3. **Importación:** Conversión de abundancias a conteos a nivel de gen mediante `tximport`.
4. **Análisis Estadístico:** Identificación de DEG y normalización con `DESeq2`.
5. **Análisis de Coexpresión:** Construcción de redes de interacción génica con `igraph`.
6. **Enriquecimiento Funcional:** Interpretación de términos GO y rutas KEGG con `gprofiler2`.

## 📊 Visualización de Resultados

El pipeline genera las siguientes representaciones gráficas fundamentales:
* **MA-Plot:** Visualización de la distribución de la expresión y cambios logarítmicos (`DESeq2`).
* **Heatmap:** Patrones de expresión con clustering jerárquico (`pheatmap`).
* **Volcano Plot:** Relación entre significancia estadística y magnitud del cambio (`ggplot2`).
* **Red de Coexpresión:** Visualización de la arquitectura de la red génica (`igraph`).

## 🛠 Herramientas y Bibliotecas Utilizadas

| Herramienta / Librería | Función en este estudio |
| :--- | :--- |
| **FastQC** | Control de calidad de secuencias. |
| **Salmon / tximport** | Cuantificación e importación de datos. |
| **DESeq2** | Análisis estadístico de expresión diferencial. |
| **gprofiler2** | Enriquecimiento funcional (GO/KEGG). |
| **igraph** | Generación y análisis de redes. |
| **pheatmap / ggplot2** | Visualización avanzada de datos. |
| **dplyr** | Manipulación y limpieza de datos. |

---
**Autor:** Oriana Batista Ceballos (2025)
