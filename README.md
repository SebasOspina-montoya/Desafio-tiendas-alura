# Proyecto: Análisis de Tiendas para Decisión de Inversión

## 📌 Descripción del proyecto

Este proyecto tiene como objetivo analizar el rendimiento de cuatro tiendas con base en distintos criterios cuantitativos para determinar cuál tienda presenta el peor desempeño y, por lo tanto, debería ser vendida.

El análisis considera factores clave como:

* Ingresos totales
* Ventas por categoría
* Calificación promedio de clientes
* Productos más y menos vendidos
* Costo de envío promedio
* Ponderación final por criterios

Se desarrollaron visualizaciones y una calificación ponderada final para respaldar la decisión.

---

## 📂 Estructura del proyecto

```
📦 proyecto-tiendas
├── data/                # Datos fuente
├── notebooks/           # Google Colab / Jupyter Notebooks
├── images/              # Gráficos exportados
├── README.md            # Este archivo
```

---

## ✅ Objetivos

1. Analizar el desempeño global de cada tienda usando criterios relevantes.
2. Visualizar métricas clave mediante gráficos.
3. Asignar una calificación ponderada final por tienda.
4. Recomendar la tienda que debe venderse basándose en los resultados.

---

## 📊 Variables analizadas

| Criterio                     | Descripción                      |
| ---------------------------- | -------------------------------- |
| Análisis de facturación      | Evalúa ingresos de la tienda     |
| Ventas por categoría         | Medición por categoría relevante |
| Calificación promedio        | Satisfacción del cliente         |
| Productos más/menos vendidos | Rotación del portafolio          |
| Envío promedio               | Costo/logística                  |

---

## 🧮 Metodología

1. **Creación del DataFrame** con puntajes por tienda.
2. **Asignación de pesos** por criterio.
3. **Cálculo de Score Final:**

```
score_final = sumatoria(valor_criterio * peso)
```

4. **Ordenamiento de tiendas según score final.**
5. **Recomendación final.**

---

## 🧾 Tabla de calificaciones

| Tienda   | Facturación | Categorías | Cal. Promedio | Productos | Envío | Cal. Final |
| -------- | ----------- | ---------- | ------------- | --------- | ----- | ---------- |
| Tienda 1 | 5           | 2          | 2             | 5         | 2     | 3.65       |
| Tienda 2 | 4           | 5          | 4             | 5         | 3     | 3.90       |
| Tienda 3 | 3           | 4          | 5             | 5         | 4     | 3.75       |
| Tienda 4 | 2           | 3          | 3             | 4         | 5     | 2.95       |

---

## 📈 Gráficos

Se generaron gráficos comparativos:


* Ventas por tienda

  <img width="481" height="504" alt="Grafico porcentaje de facturacion por tienda" src="https://github.com/user-attachments/assets/b2ebe0ba-30d1-4027-a7b2-7cda23278e33" />
  
* Calificacion promedio clientes

  <img width="554" height="374" alt="Grafico Calificacion promedio clientes" src="https://github.com/user-attachments/assets/bbc8054c-c138-4618-bb40-d53ba240ec0a" />
  
* Grafico calificacion final de las tiendas

  
  <img width="516" height="528" alt="Grafico Calificacion de las tiendas" src="https://github.com/user-attachments/assets/84ac16af-bcca-40b7-af65-8320793beeb7" />
  


## ✅ Conclusión

De acuerdo con el análisis ponderado, **la tienda que debe venderse es la Tienda 4**, ya que presenta el score final más bajo debido principalmente a su baja facturación y desempeño general.

---

## 🛠️ Requerimientos

```
pandas
matplotlib
```
## ✍️ Autor

* **Sebastián Ospina**

---

## 📄 Licencia

Este proyecto es de uso libre con fines educativos.
