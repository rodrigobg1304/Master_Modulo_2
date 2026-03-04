# 🎯 Análisis Predictivo LaLiga: Big Data en Fútbol

**Actividad Módulo 2 - Máster Big Data e IA en el Deporte**  
Proyecto completo de análisis predictivo sobre datos ficticios de **760 partidos de LaLiga** (temporadas 2023/24 y 2024/25). Generación de dataset, EDA, limpieza, modelado y recomendaciones estratégicas.[file:1][file:3]

[![LaLiga Predictive Analysis](https://img.shields.io/badge/Tech-Python%20%7C%20Pandas%20%7C%20Scikit--learn%20%7C%20Matplotlib-brightgreen)](https://www.python.org/) [![Score](https://img.shields.io/badge/Score-8.5%2F10-orange.svg)](https://github.com/rodrigobg1304/Master_Modulo_2)

## 📊 Resumen del Proyecto

Simulación realista de **LaLiga** con **20 equipos**, **38 jornadas** por temporada y **44 features** por partido (goles, xG, tiros, posesión, duelos, disciplina, etc.). Dataset generado con IA para coherencia con datos reales (inspirado en Sofascore).[file:1][file:3]

### Metodología aplicada
1. **Generación datos ficticios** ✅ (760 registros)
2. **EDA y limpieza** ✅ (1.57% nulos tratados con KNN, medianas por equipo, proporciones)
3. **Modelado predictivo** ✅ (Regresión lineal, Logística, Random Forest, CV 5-fold)
4. **Evaluación** ✅ (R², MAE, RMSE, Accuracy, F1, ROC-AUC)
5. **Informe final** ✅ (Recomendaciones tácticas y estratégicas)

## 🔍 Modelos desarrollados

| Modelo | Objetivo | Métricas clave (Test) | Observaciones |
|--------|----------|-----------------------|---------------|
| **Regresión Lineal** | Puntos por temporada | R²=0.435, MAE=4.66 | Sobreajuste detectado, inestable en CV |
| **Regresión Logística** | Over/Under 2.5 goles | Accuracy ~100%, ROC-AUC perfecto | Muy robusto, clases balanceadas (51/49%)[file:1] |
| **Random Forest** | Over/Under 2.5 goles | Similar a Logística | Alta precisión, pocos errores |

**Insights clave**: Precisión de pases y posesión influyen negativamente en goles; tiros a puerta y paradas son drivers principales.[file:1]

## 📈 Resultados destacados

- **Dataset limpio**: Listo para producción tras manejo inteligente de outliers y nulos.
- **Mejor modelo**: Logística para predicción de goles (matriz confusión: 4 FN, 0 FP).
- **Recomendaciones**:
  - **Táctica**: Estrategias agresivas en partidos "Over" (alta presión, volumen tiro).
  - **Scouting**: Priorizar perfiles ofensivos en equipos de ataque; defensivos en control.

## 📁 Estructura del repositorio

├── 📁 input/
│ ├── football_matches_dataset.csv # Dataset original (con nulos)
│ └── football_matches_dataset_clean.csv # Dataset procesado
├── 📄 Actividad_M2_Analysis.ipynb # EDA, modelado y evaluación
├── 📄 Actividad Modulo 2.pdf # Informe completo
└── 📄 README.md # Este archivo

📚 Recursos y referencias
- Inspiración datos: Sofascore
- Autor: Rodrigo Benito García | Madrid, España | Marzo 2026

