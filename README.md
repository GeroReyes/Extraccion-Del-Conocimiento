# Proyecto de Extracción de Conocimiento en Bases de Datos (KDD)

**Nombre del alumno:** Juan Gerardo Reyes Carrera

**Materia:** Extracción de Conocimiento en Bases de Datos  

**Cuatrimestre:** 9° Cuatrimestre  

---

## Descripción general

Este proyecto aplica el proceso estándar de **Extracción de Conocimiento en Bases de Datos (KDD)** sobre una base de datos relacional de una tienda minorista ficticia. Se siguen las etapas clásicas: selección, preprocesamiento, transformación, minería de datos e interpretación/evaluación. El objetivo final es descubrir patrones de compra, segmentar clientes y generar reglas de asociación que permitan mejorar estrategias de marketing y ventas cruzadas.

---

## Objetivo

Extraer conocimiento no trivial, implícito y potencialmente útil a partir de una base de datos transaccional, mediante técnicas de minería de datos (reglas de asociación y clustering), para identificar perfiles de clientes y productos con alta co-ocurrencia en las compras.

---

## Datasets utilizados

Se parte de una **base de datos relacional** en formato SQLite con tres tablas principales:

| Tabla         | Descripción | Registros aproximados |
|---------------|-------------|----------------------|
| `clientes`    | Datos demográficos (ID, edad, ciudad, nivel socioeconómico) | 5000 |
| `productos`   | Catálogo (ID producto, categoría, precio, costo) | 200 |
| `transacciones` | Ventas (ID transacción, ID cliente, ID producto, fecha, cantidad) | 50,000 |

**Fuente:** Dataset sintético generado con `mockaroo` y ajustado manualmente para simular estacionalidades y patrones de compra.

---

## Herramientas utilizadas

| Herramienta       | Propósito en el proyecto |
|-------------------|--------------------------|
| **SQLite**        | Base de datos original y consultas iniciales |
| **Pandas**        | Extracción, limpieza y transformación de datos |
| **NumPy**         | Operaciones vectoriales y transformaciones numéricas |
| **Scikit-learn**  | Algoritmos de clustering (K-Means) y preprocesamiento |
| **Apyori**        | Implementación de reglas de asociación (Apriori) |
| **Matplotlib / Seaborn** | Visualización de patrones y clusters |
| **Jupyter Notebook** | Entorno interactivo para documentar el proceso KDD |
| **SQLAlchemy**    | Conexión entre Python y SQLite |

---

## Instrucciones de ejecución general

### 1. Clonar el repositorio
```bash
git clone https://github.com/usuario/proyecto-kdd.git
cd proyecto-kdd
