# Ciencia de los Materiales

Proyecto de la asignatura **Ciencia de los Materiales**: simulación de Montecarlo del modelo de Ising 2D y de la ecuación TDGL (Time-Dependent Ginzburg–Landau).

**Autora:** Natalia Isabel Martinez

## Contenido

| Archivo | Descripción |
|---|---|
| `Simulacion_Montecarlo_Ising_2D.ipynb` | Notebook principal (Google Colab) |

El notebook tiene cuatro partes:

1. **Transición de fase del modelo de Ising 2D.** Algoritmo de Metropolis en una red N×N con condiciones de frontera periódicas. Barre la temperatura (T de 1.53 a 3.28) y calcula energía, magnetización, calor específico y susceptibilidad.
2. **Evolución de la configuración de espines.** Red de 64×64 a baja temperatura; muestra cómo se forman los dominios magnéticos a lo largo de los barridos de Montecarlo.
3. **Ecuación TDGL.** Integración con Euler explícito usando un laplaciano en matriz dispersa (`scipy.sparse`) para ver la separación de fases.
4. **TDGL con parámetros ajustados.** Versión mejorada de la anterior, con mapa de colores `bwr` en el rango [-1, 1].

## Cómo ejecutarlo

Ábrelo en [Google Colab](https://colab.research.google.com/) (Archivo → Subir notebook) o localmente con Jupyter:

```bash
pip install numpy scipy matplotlib
jupyter notebook Simulacion_Montecarlo_Ising_2D.ipynb
```
