## 📊 El Conjunto de Datos (Dataset)

El proyecto utiliza el dataset público de Kaggle **Chest X-Ray Images (Pneumonia)**, el cual consta de **imágenes de rayos X de tórax (JPEG)** divididas en dos categorías: **Pneumonia** (Neumonía) y **Normal**.

---

## 🔗 Origen de los Datos

El conjunto de datos utilizado en este proyecto es público y se puede descargar directamente desde la plataforma Kaggle a través del siguiente enlace:

📌 **Dataset:** [Chest X-Ray Images (Pneumonia) en Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia/data)

> ⚠️ **Nota:** Debido a las restricciones de tamaño de GitHub (5,863 imágenes en formato JPEG), los archivos del dataset no están incluidos en este repositorio. Es necesario descargarlos desde el enlace anterior y posicionarlos en la estructura de carpetas indicada abajo.

---

### 🔍 Características y Rigor Médico

* **Origen:** Las radiografías de tórax (proyección anterior-posterior) pertenecen a cohortes retrospectivas de pacientes pediátricos de 1 a 5 años del *Guangzhou Women and Children’s Medical Center*.
* **Control de Calidad:** Todas las imágenes pasaron por un filtro previo donde se eliminaron los escaneos de baja calidad o ilegibles.
* **Validación de Expertos:** Los diagnósticos fueron etiquetados y calificados originalmente por dos médicos expertos antes de ser aprobados para el entrenamiento. Para eliminar errores de sesgo, el conjunto de evaluación (*test*) fue verificado además por un tercer médico experto.
