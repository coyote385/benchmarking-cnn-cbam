## 📊 El Conjunto de Datos (Dataset)

El proyecto utiliza el dataset médico de referencia pública **LIDC-IDRI** (*Lung Image Database Consortium and Image Database Resource Initiative*), el cual consiste en exploraciones de **Tomografía Computarizada (TC) de tórax** en formato DICOM para la detección, diagnóstico y clasificación de nódulos pulmonares y cáncer de pulmón.

---

## 🔗 Origen de los Datos

El conjunto de datos es administrado por *The Cancer Imaging Archive (TCIA)* y se encuentra disponible públicamente para fines de investigación:

📌 **Dataset:** [LIDC-IDRI en The Cancer Imaging Archive (TCIA)](https://doi.org/10.7937/K9/TCIA.2015.LO9QL9SX)

> ⚠️ **Nota:** Debido al gran volumen de datos (imágenes volumétricas en formato DICOM de 1,018 casos), los archivos originales no se alojan en este repositorio. Es necesario descargarlos directamente mediante la herramienta *NBIA Data Retriever* desde TCIA y organizarlos en la estructura de carpetas definida en este proyecto.

---

### 🔍 Características y Rigor Médico

- **Origen y Cobertura:** Desarrollado por siete instituciones académicas e industrias de imágenes médicas en un esfuerzo conjunto liderado por el *National Cancer Institute (NCI)*.
- **Volumen de Datos:** Contiene **1,018 casos (estudios de TC de tórax)** de pacientes con presencia confirmada o sospecha de nódulos pulmonares.
- **Validación Multiexperto:** Cada estudio fue evaluado en un proceso de dos fases por cuatro radiólogos torácicos experimentados. Los expertos identificaron, localizaron y anotaron detalladamente los nódulos (características morfológicas y nivel de malignidad).
- **Referencia Bibliográfica:**
  > Armato III, S. G., McLennan, G., Bidaut, L., McNitt-Gray, M. F., Meyer, C. R., Reeves, A. P., ... & Clarke, L. P. (2011). *The Lung Image Database Consortium (LIDC) and Image Database Resource Initiative (IDRI): A completed reference database of lung nodules on CT scans.* **Medical Physics**, 38(2), 915-931. https://doi.org/10.1118/1.3528204
```<ElicitationsGroup message="¿Deseas complementar alguna otra parte del README para este nuevo dataset?">
  <Elicitation label="Generar estructura de carpetas para procesar datos DICOM/LIDC-IDRI" query="¿Puedes ayudarme a redactar la sección de estructura de carpetas y preprocesamiento de imágenes DICOM para el README.md?"/>
  <Elicitation label="Redactar sección de Metodología y Arquitectura CNN + CBAM" query="¿Puedes ayudarme a redactar la sección de Metodología y Modelo (CNN + CBAM) para el README.md?"/>
</ElicitationsGroup>
