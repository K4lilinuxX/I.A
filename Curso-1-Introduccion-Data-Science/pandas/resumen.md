## 📝 Resumen de Aprendizaje: Análisis de Datos (Titanic)
Aquí documento los conceptos clave y técnicas que he dominado durante el análisis del dataset del Titanic.

**🚀 Conceptos y Técnicas Dominadas**
1. Agregación y Análisis Estadístico

* `groupby()`: Aprendí a agrupar datos por categorías (ej. `Pclass` o `Survived`) para realizar cálculos específicos.

* Cálculo de Proporciones: Comprendí que, con variables binarias (0 y 1), el `mean()` (promedio) equivale directamente a la tasa porcentual.

Ejemplo: `df.groupby("Pclass")["Survived"].mean() * 100`

2. Manipulación de Datos Continuos

* Binning (`pd.cut` / `pd.qcut`): Aprendí a transformar variables numéricas continuas (como `Fare` o `Age`) en categorías discretas para facilitar su análisis y visualización.

* Aprendizaje clave: Uso de `np.inf` para manejar rangos abiertos (ej. "100+") y asegurar que el código no falle con datos nuevos.

3. Visualización de Datos

* Gráficas de Barras: Dominé el uso de `plt.bar` para comparar tasas de supervivencia.

* Personalización de Ejes: Aprendí a usar `plt.xticks()` con ticks y labels para limpiar el eje X y reemplazar códigos numéricos por etiquetas claras ("Sobrevivió" / "No sobrevivió").

* Buenas Prácticas: Entendí la importancia de incluir etiquetas, títulos, leyendas (`plt.legend`) y rejillas (`plt.grid`) para que las gráficas sean profesionales.

**💡 Interpretación de Resultados (Insights)**
* Estratificación Socioeconómica: Confirmé que el precio del boleto tiene una correlación positiva con la supervivencia. Los pasajeros con boletos de mayor valor tuvieron mayores probabilidades de sobrevivir, evidenciando una diferencia en el acceso a recursos de seguridad.

* Calidad vs. Cantidad: Aprendí que graficar "media de precios" es una forma efectiva de detectar brechas económicas entre grupos (sobrevivientes vs. no sobrevivientes).

**🛠 Próximos Pasos**
* [ ] Aplicar técnicas de manejo de valores nulos (NaN).

* [ ] Explorar la variable Sex para confirmar la hipótesis de "prioridad en la evacuación".

* [ ] Aprender Seaborn para gráficas con estilos más modernos.