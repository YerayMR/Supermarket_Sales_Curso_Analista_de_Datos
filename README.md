# 🛒 Supermarket Sales – Análisis de Datos y Dashboard en Excel

Este proyecto consiste en aplicar el flujo completo de análisis de datos utilizando **Microsoft Excel**, desde la importación y preparación del dataset hasta la creación de un **dashboard interactivo** con tablas dinámicas, segmentadores y KPIs.

El objetivo es transformar datos brutos en información comprensible y accionable, siguiendo buenas prácticas de análisis y diseño visual.

**Dataset utilizado:**  
📌 *Supermarket Sales* – Kaggle  
🔗 https://www.kaggle.com/datasets/faresashraf1001/supermarket-sales

El dataset contiene información realista de ventas en supermercados, incluyendo fecha, producto, categoría, método de pago, ciudad, cantidad, impuestos y totales.

---

## ⚠️ Notas Previas sobre el Formato del Dataset

El archivo original del dataset *Supermarket Sales* está en **formato numérico anglosajón**, lo que implica:

- Uso de **punto (.) como separador decimal**
- Uso de **coma (,) en la estructura del CSV**
- Ausencia de separadores de miles
- Valores numéricos como: `74.69`, `26.1415`, `548.9715`, etc.

### ❗ Problema en Excel Web
Excel Web **no interpreta correctamente** los decimales anglosajones.  
Al intentar convertir las columnas numéricas, Excel:

- Elimina el punto decimal original  
- Convierte `26.1415` en `261415`  
- Lo reformatea como `261.415`  
- Daña la precisión y estructura del dato  
- Hace imposible recuperar el número original  

Esto ocurre porque Excel Web fuerza automáticamente el formato numérico europeo al dividir texto en columnas o cambiar el tipo de celda.

### ✔️ Solución recomendada antes de importar
Para evitar la pérdida de datos, es necesario **convertir los decimales antes de que Excel procese el archivo**. Existen tres alternativas seguras:

1. **Abrir el CSV en un editor de texto** y reemplazar:
   - `,` → `;`  
   - `.` → `,`  
   Luego guardar como CSV UTF-8.

2. **Importar el CSV en Google Sheets**, que sí respeta los decimales, y después:
   - Archivo → Descargar → Microsoft Excel  
   El archivo resultante mantiene los números correctos.

3. **Abrir el archivo directamente en Excel Escritorio**  
   (si está disponible), donde Power Query permite importar correctamente el formato anglosajón.

### ✔️ Resultado esperado tras la corrección
Una vez formateado el CSV de forma adecuada:

- `74.69` → `74,69`
- `26.1415` → `26,1415`
- `548.9715` → `548,9715`

Conservando exactamente los valores originales y permitiendo:

- Calcular correctamente las tablas dinámicas  
- Construir KPIs fiables  
- Realizar análisis estadístico válido  

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

