# seaborn

Seaborn incluye varios tipos de gráficos para diferentes tipos de análisis. Algunos de los más comunes son:


   ¡ Gráficos de dispersión (scatterplot): Muestra la relación entre dos variables cuantitativas.

   ¡ Gráficos de líneas (lineplot): Ideal para mostrar tendencias a lo largo del tiempo.

   ¡ Histogramas (histplot): Útiles para mostrar la distribución de una variable.

   ¡ Gráficos de barras (barplot): Muestra la media de una variable categórica, con intervalos de confianza.

   ¡ Boxplots (boxplot): Representa la distribución de una variable numérica agrupada por una variable categórica.

   ¡ Gráficos de violín (violinplot): Similar a los boxplots, pero también muestra la densidad de los datos.

   ¡ Pairplot: Muestra todas las combinaciones posibles de gráficos de dispersión entre pares de variables.

   ¡ Heatmaps: Ideal para mostrar matrices de correlación o datos en formato de tabla.

   # Estilos para una Presentación Más Profesional

Seaborn permite personalizar los estilos de los gráficos para que se vean más elegantes y profesionales. Aquí algunos consejos:

# Configurar el estilo:
import seaborn as sns
sns.set_style("whitegrid")

# Paletas de colores:
palette = sns.color_palette("deep")

# Ajustar la escala: 
sns.set_context("talk")

# Añadir títulos y etiquetas:
import matplotlib.pyplot as plt
plt.title("Mi Gráfico Profesional")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")

# Guardar gráficos:
plt.savefig("grafico_profesional.png", dpi=300)

# Ejemplo de Código: 

import seaborn as sns
import matplotlib.pyplot as plt

# Cargar datos de ejemplo
tips = sns.load_dataset("tips")

# Configurar el estilo
sns.set_style("whitegrid")
sns.set_context("talk")

# Crear un gráfico de barras
plt.figure(figsize=(10, 6))
sns.barplot(x="day", y="total_bill", data=tips, palette="deep")

# Personalizar título y etiquetas
plt.title("Promedio de Total de Cuenta por Día")
plt.xlabel("Día de la Semana")
plt.ylabel("Total de Cuenta Promedio")

# Mostrar el gráfico
plt.show()




