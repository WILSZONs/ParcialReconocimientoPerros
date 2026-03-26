## 📉 Conclusiones del Experimento: CNN "Since Zero"

Tras entrenar una arquitectura de Red Neuronal Convolucional (CNN) propia para clasificar **120 razas de perros**, se determinó que el enfoque es **inviable** bajo las condiciones actuales.

### 📊 Resumen de Métricas Finales
| Métrica | Entrenamiento | Validación | Azar (Base) |
| :--- | :---: | :---: | :---: |
| **Accuracy** | 11.09% | **6.43%** | 0.83% |
| **Loss** | 3.87 | 4.24 | - |

### ⚠️ Análisis de Limitaciones

1.  **Complejidad del Dataset (120 clases):** El modelo se enfrentó a un problema de clasificación de grano fino (*fine-grained classification*). Diferenciar entre 120 categorías requiere una profundidad y una extracción de características que una CNN pura y simple no logra alcanzar, resultando en una incapacidad para converger.
2.  **Rendimiento Insuficiente:** Aunque el modelo rinde ligeramente mejor que una elección aleatoria (~6% vs 0.83%), el **accuracy es extremadamente bajo** para cualquier uso práctico. No fue posible "montar" un modelo que realmente aprendiera a distinguir las razas.
3.  **Sobreajuste y Divergencia:** Las gráficas muestran que, mientras la pérdida en entrenamiento bajaba, la de validación se estancaba o subía. Esto indica que el modelo memor
