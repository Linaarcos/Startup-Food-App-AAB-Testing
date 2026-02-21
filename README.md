# 🛒 Análisis de Conversión y Test A/A/B - Startup Alimentaria

## 📖 Introducción
En este proyecto, analicé el comportamiento de los usuarios de una startup de productos alimenticios. El objetivo fue doble: primero, entender el **embudo de ventas** para optimizar la experiencia del usuario y, segundo, evaluar un experimento de diseño (cambio de fuentes) mediante un **Test A/A/B**.

## 📊 Fases del Proyecto

### 1. Preparación y Limpieza
* Transformación de timestamps a formatos de fecha/hora.
* Filtrado de datos antiguos para asegurar un análisis sobre un periodo con registros completos (agosto 2019).

### 2. Análisis del Embudo (Funnel Analysis)
* Identificación de la secuencia de eventos: `MainScreenAppear` -> `OffersScreenAppear` -> `CartScreenAppear` -> `PaymentScreenSuccessful`.
* **Hallazgo:** La mayor pérdida de usuarios ocurre en el primer paso (transición de la pantalla principal a ofertas). Solo el **47.7%** de los usuarios iniciales llega a completar un pago.

### 3. Experimento A/A/B
* **Grupos de Control (246 y 247):** Validación de que no existen diferencias significativas entre ellos (Test A/A exitoso).
* **Grupo Experimental (248):** Comparativa del nuevo diseño de fuentes contra los grupos de control.
* **Resultado:** No se hallaron diferencias estadísticamente significativas en las tasas de conversión.

## 🛠️ Stack Tecnológico
* **Python:** Lenguaje principal.
* **Pandas:** Manipulación de dataframes.
* **Plotly:** Creación de embudos interactivos.
* **SciPy:** Pruebas estadísticas de proporciones (Z-test).

## 💡 Conclusión de Negocio
Basado en los resultados del test A/A/B, el cambio de fuentes no influye negativamente (ni positivamente) en la conversión. Se recomienda a la gerencia que el equipo de diseño puede proceder con el cambio si es por una cuestión estética o de marca, ya que no representa un riesgo para las ventas.
