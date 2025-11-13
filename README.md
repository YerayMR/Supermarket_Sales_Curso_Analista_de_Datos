# 🛒 Supermarket Sales – Análisis de Datos y Dashboard en Excel

Este proyecto consiste en aplicar el flujo completo de análisis de datos utilizando **Microsoft Excel**, desde la importación y preparación del dataset hasta la creación de un **dashboard interactivo** con tablas dinámicas, segmentadores y KPIs.

El objetivo es transformar datos brutos en información comprensible y accionable, siguiendo buenas prácticas de análisis y diseño visual.

**Dataset utilizado:**  
📌 *Supermarket Sales* – Kaggle  
🔗 https://www.kaggle.com/datasets/faresashraf1001/supermarket-sales

El dataset contiene información realista de ventas en supermercados, incluyendo fecha, producto, categoría, método de pago, ciudad, cantidad, impuestos y totales.

---

## ⚠️ Notas Previas sobre el Formato del Dataset

El dataset *Supermarket Sales* utiliza **formato anglosajón**, lo que genera problemas al importarlo en **Excel Web**, que trabaja con configuración europea.

### ❗ Problemas detectados
1. **Decimales anglosajones**
   - Los números vienen con **punto (.) como separador decimal**.
   - Excel Web elimina el punto al convertir la celda a número, provocando errores como:
     - `26.1415` → `261415` → `261.415` (dato dañado).
   - Esto impide cálculos fiables y afecta a pivot tables o KPIs.

2. **Fechas en formato MM/DD/YYYY**
   - Excel Web interpreta de forma incorrecta el formato americano.
   - Algunas fechas se autoconvierten, otras quedan como texto, produciendo mezclas como:
     - `03/07/2019` interpretado como 3 de julio.
     - `12/1/2019` interpretado como 12 de enero.
   - Al convertir estas fechas a texto se pierde la forma original, haciendo imposible reconstruirlas desde Excel Web.

### 📌 Limitaciones de Excel Web
Excel Web no dispone de:
- Power Query  
- Control avanzado del tipo de dato antes de la importación  
- Herramientas para impedir la autocorrección automática de fechas y decimales  

Por tanto, procesar el CSV directamente en Excel Web provoca pérdida irreversible de información.

### ✔️ Solución adoptada
Para preservar la integridad del dataset y convertirlo correctamente al formato europeo, se realiza un **preprocesado completo en Google Colab** utilizando `pandas`, donde:

- Se interpretan correctamente los decimales anglosajones.
- Se convierten las fechas a formato estándar europeo.
- Se exporta un archivo limpio a `.xlsx` o `.csv` listo para trabajar en Excel Web.

Este preprocesado garantiza que el análisis, las tablas dinámicas y el dashboard funcionen sin errores.

---

## 🎯 Objetivos del Proyecto

1. Importar, limpiar y preparar datos.  
2. Realizar análisis exploratorio básico.  
3. Crear métricas y transformaciones simples.  
4. Construir análisis avanzado mediante tablas dinámicas.  
5. Diseñar un dashboard profesional e interactivo.  
6. Opcional: aplicar transformaciones avanzadas con Power Query (solo Excel escritorio).

---

# 🏆 Niveles de Entrega (Checklist Completo)

Marca ✔️ cuando completes cada apartado.  
Si no lo realizas, marca ❌.

---

## 🟢 Nivel Esencial

| Tarea | Estado |
|-------|--------|
| Datos importados y convertidos en tabla de Excel | ⬜ ✔️ / ❌ |
| Eliminación de duplicados | ⬜ ✔️ / ❌ |
| Filtrado y ordenación cronológica | ⬜ ✔️ / ❌ |
| Formato condicional aplicado para un análisis básico | ⬜ ✔️ / ❌ |
| Creación de nuevas columnas con funciones básicas (ej. SI) | ⬜ ✔️ / ❌ |
| Análisis estadístico descriptivo (herramienta de análisis de datos) | ⬜ ✔️ / ❌ |

---

## 🟡 Nivel Medio

| Tarea | Estado |
|-------|--------|
| Uso completo de tablas dinámicas | ⬜ ✔️ / ❌ |
| Creación de gráficos basados en tablas dinámicas | ⬜ ✔️ / ❌ |
| Diseño del dashboard (formas, títulos, estructura) | ⬜ ✔️ / ❌ |
| KPIs creados y vinculados dinámicamente a tablas | ⬜ ✔️ / ❌ |

---

## 🟠 Nivel Avanzado

| Tarea | Estado |
|-------|--------|
| Dashboard interactivo mediante segmentadores | ⬜ ✔️ / ❌ |
| Segmentadores conectados a todas las tablas dinámicas | ⬜ ✔️ / ❌ |
| Formato visual tipo “aplicación” (pantalla completa, ocultar cuadrícula…) | ⬜ ✔️ / ❌ |

---

## 🔴 Nivel Experto *(Opcional – requiere Excel de escritorio)*

| Tarea | Estado |
|-------|--------|
| Ocultar completamente interfaz de Excel (barras, pestañas, scroll) | ⬜ ✔️ / ❌ |
| Transformaciones avanzadas con Power Query | ⬜ ✔️ / ❌ |
| Archivo capaz de actualizar datos con mínima intervención | ⬜ ✔️ / ❌ |

---

## 📊 Resultado Final Esperado

- Un **dashboard interactivo**, claro y funcional.  
- Posibilidad de filtrar ventas por ciudad, categoría, método de pago, fecha y más.  
- KPIs dinámicos como:
  - Ventas totales  
  - Ticket promedio  
  - Ingresos por categoría  
  - Impuestos generados  
- Hoja oculta con todas las tablas dinámicas utilizadas.

---

## 📘 Notas del Autor

Este README está preparado para guiar el desarrollo paso a paso.  
Cada sección marcada con ❌ puede completarse más adelante y actualizarse fácilmente.

