## 🚗 Análisis del Dataset *mtcars*

El dataset **mtcars** contiene información sobre **32 modelos de autos** (años 1973–74) y **11 variables numéricas** relacionadas con su **rendimiento, consumo y diseño mecánico**.

### 📋 Descripción de las variables principales

| Variable | Descripción | Tipo | 
|-----------|--------------|------|
| **mpg** | Millas por galón (eficiencia) | numérica |
| **cyl** | Número de cilindros | entera 
| **disp** | Desplazamiento (pulg³) | numérica |
| **hp** | Caballos de fuerza | numérica |
| **drat** | Relación del eje trasero | numérica | 
| **wt** | Peso (miles de libras) | numérica | 
| **qsec** | Tiempo 1/4 de milla (segundos) | numérica | 
| **vs** | Tipo de motor (0 = en V, 1 = recto) | binaria |
| **am** | Transmisión (0 = automática, 1 = manual) | binaria | 
| **gear** | Cantidad de marchas | entera |
| **carb** | Cantidad de carburadores | entera |

---

### 📊 Relaciones entre variables

#### 🔹 Relación con la eficiencia (mpg)
- Las variables más relacionadas con el **consumo (mpg)** son:
  - **Número de cilindros**, **peso** y **desplazamiento**, todas con correlaciones negativas cercanas al **-85%**, indicando que autos más pesados o con motores más grandes consumen más combustible.  
  - **Caballos de fuerza** y **tipo de motor (vs)** muestran correlaciones positivas (≈ +68%), asociadas a un mejor rendimiento.

#### 🔹 Correlaciones entre variables técnicas
- **Cilindros ↔ Desplazamiento:** 0.90  
- **Peso ↔ Desplazamiento:** 0.89  
- **Cilindros ↔ Caballos de fuerza:** 0.83  
- **Cilindros ↔ Tipo de motor:** 0.81  

---

### 💡 Insights clave

- 🔸 Los autos **manuales** y con **motor en línea** tienden a ser **más eficientes**.  
- 🔸 Una **menor cantidad de cilindros, peso y desplazamiento** implica **mayor eficiencia**.  
- 🔸 La **cantidad de marchas** y la **relación del eje trasero** se asocian a un mejor rendimiento.  
- 🔸 Los autos con **más caballos de fuerza o más carburadores** suelen tener **menor eficiencia de combustible**.

---

### 🤖 Modelos predictivos para mpg

| Modelo | R² | RMSE | MAE |
|--------|----|------|------|
| **Random Forest** | **0.717** | **1.888** | **1.766** |
| **SVM** | 0.704 | 1.932 | 1.618 |
| **Gradient Boost** | 0.692 | 1.972 | 1.854 |
| **MLP (Neural Network)** | 0.439 | 2.659 | 2.167 |

📈 **El modelo Random Forest logra el mejor desempeño**, con un R² de 0.717 y un RMSE inferior a 1.9, mostrando buena capacidad para predecir la eficiencia (mpg) en base a las características del auto.

---
