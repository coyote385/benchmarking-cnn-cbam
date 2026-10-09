# Evaluación Comparativa: CNN Tradicional vs. CNN con Módulo de Atención CBAM para la Clasificación de Cáncer de Pulmón en Imágenes de TC

## Introducción

El cáncer de pulmón es una de las causas principales de mortalidad por cáncer a nivel mundial. El diagnóstico temprano es crucial para mejorar las tasas de supervivencia de los pacientes; sin embargo, la detección manual de nódulos pulmonares sospechosos en estudios de **Tomografía Computarizada (TC) de tórax** representa un desafío considerable para los radiólogos debido al alto volumen de cortes por estudio, la variabilidad morfométrica de las lesiones y la presencia de estructuras anatómicas complejas.

En los últimos años, los sistemas de **Diagnóstico Asistido por Computadora (CAD)** basados en **Redes Neuronales Convolucionales (CNN)** han demostrado un rendimiento sobresaliente en el procesamiento de imágenes médicas. No obstante, las arquitecturas convolucionales convencionales suelen tratar las características espaciales y de canales con igual ponderación, lo que puede limitar su capacidad para focalizarse en regiones patológicas sutiles o pequeñas.

Para abordar esta limitación, este proyecto propone una **evaluación comparativa entre una arquitectura CNN tradicional y una arquitectura optimizada con el Módulo de Atención Convolucional de Bloque (CBAM - *Convolutional Block Attention Module*)**. El mecanismo de atención CBAM permite a la red enfatizar de forma adaptativa *qué* características son relevantes (atención de canal) y *dónde* se localizan las regiones de interés anatómico (atención espacial), mejorando la precisión y la capacidad discriminativa en la clasificación de nódulos pulmonares.

## El Conjunto de Datos (Dataset)

El proyecto utiliza el dataset médico de referencia pública **LIDC-IDRI** (*Lung Image Database Consortium and Image Database Resource Initiative*), el cual consiste en exploraciones de **Tomografía Computarizada (TC) de tórax** en formato DICOM para la detección, diagnóstico y clasificación de nódulos pulmonares y cáncer de pulmón.

---

## 🔗 Origen de los Datos

El conjunto de datos es administrado por *The Cancer Imaging Archive (TCIA)* y se encuentra disponible públicamente para fines de investigación:

**Dataset:** [LIDC-IDRI en The Cancer Imaging Archive (TCIA)](https://doi.org/10.7937/K9/TCIA.2015.LO9QL9SX)

> ⚠️ **Nota:** Debido al gran volumen de datos (imágenes volumétricas en formato DICOM de 1,018 casos), los archivos originales no se alojan en este repositorio. Es necesario descargarlos directamente mediante la herramienta *NBIA Data Retriever* desde TCIA y organizarlos en la estructura de carpetas definida en este proyecto.

---

### 🔍 Características y Rigor Médico

- **Origen y Cobertura:** Desarrollado por siete instituciones académicas e industrias de imágenes médicas en un esfuerzo conjunto liderado por el *National Cancer Institute (NCI)*.
- **Volumen de Datos:** Contiene **1,018 casos (estudios de TC de tórax)** de pacientes con presencia confirmada o sospecha de nódulos pulmonares.
- **Validación Multiexperto:** Cada estudio fue evaluado en un proceso de dos fases por cuatro radiólogos torácicos experimentados. Los expertos identificaron, localizaron y anotaron detalladamente los nódulos (características morfológicas y nivel de malignidad).
- **Referencia Bibliográfica:**
  > Armato III, S. G., McLennan, G., Bidaut, L., McNitt-Gray, M. F., Meyer, C. R., Reeves, A. P., ... & Clarke, L. P. (2011). *The Lung Image Database Consortium (LIDC) and Image Database Resource Initiative (IDRI): A completed reference database of lung nodules on CT scans.* **Medical Physics**, 38(2), 915-931. https://doi.org/10.1118/1.3528204
