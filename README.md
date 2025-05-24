
# Análisis Exploratorio de Datos de Jugadores FIFA 19  
**Autor:** Juan David Montoya Agudelo

## Descripción del Proyecto  
Este proyecto realiza un análisis exploratorio del conjunto de datos de jugadores del videojuego FIFA 19. El objetivo principal es identificar patrones y relaciones entre variables que expliquen el valor de mercado de los jugadores, sus posiciones, nacionalidades y potencial de mejora. Se utilizaron herramientas de Python como Pandas, Seaborn y Matplotlib para el tratamiento de datos, visualización y obtención de hallazgos clave.

---

## Archivos  

- `fifa_eda.csv` : Conjunto de datos de jugadores FIFA 19.  
- `fifa_analysis.ipynb` : Cuaderno Jupyter con todo el proceso de limpieza, transformación y visualización.  
- `README.md` : Este documento.  

---

## Análisis Realizado  

Se exploraron variables clave como:  

- **Valor de mercado (`Value`)**  
- **Rendimiento actual (`Overall`) y potencial (`Potential`)**  
- **Nacionalidad (`Nationality`) y posición (`Position`)**  

Se creó una variable derivada:  
- `Potential_Gap`, definida como la diferencia entre el potencial y el rendimiento actual, para observar el margen de mejora de los jugadores.

Se implementaron varias visualizaciones:  

- **Gráfico de barras del Potential_Gap**: Inicialmente se intentó graficar todos los jugadores, pero por la cantidad de datos, se filtraron los 10 con mayor diferencia.  
- **Gráfico de nacionalidades**: Se graficaron las 10 nacionalidades más frecuentes para evitar saturación visual.  
- **Boxplot del valor por posición específica**: Permitió observar la dispersión del valor de mercado entre posiciones como ST, CM, GK, etc.  
- **Boxplot del valor por tipo de posición**: Se agruparon las posiciones en categorías más amplias (Delantero, Mediocampista, Defensa, Portero), mejorando la claridad visual.

---

## Hallazgos  

- La mayoría de los jugadores tienen una brecha pequeña entre su rendimiento actual y su potencial.  
- Los **delanteros** tienden a tener un **valor de mercado más alto** que otros tipos de jugadores.  
- **Brasil, Francia y Alemania** están entre las nacionalidades más frecuentes.  
- Los **valores de mercado muestran alta dispersión** en casi todas las posiciones, con muchos valores atípicos.  
- Las posiciones defensivas y de portero tienden a tener menor valor de mercado que mediocampistas y delanteros.

---

## Observaciones  

- Se identificó una **alta cantidad de outliers**, especialmente en los valores de mercado, que podrían afectar el análisis si no se gestionan adecuadamente.  
- Algunas posiciones muy específicas (como RCM, LF, etc.) tenían muy pocos datos, por lo que fueron agrupadas para obtener mejores conclusiones.  

---

## Conclusiones  

Este análisis proporciona una visión general del mercado de jugadores en FIFA 19, destacando diferencias relevantes según la posición, el país y el potencial. Sirve como punto de partida para aplicar modelos predictivos que estimen el valor de un jugador o identifiquen talentos con alto margen de crecimiento. Se recomienda manejar mejor los outliers y considerar técnicas avanzadas como clustering o modelos de regresión para un análisis más profundo.
