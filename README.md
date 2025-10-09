# FODA del Equipo de Liderazgo Informático — Análisis Integral

Este repositorio contiene el **formulario**, el **cuadernillo Jupyter** y utilidades para analizar un **FODA por participante** y por equipo, combinando:
- **Preguntas cerradas** (escala 1–5 → normalizadas 0–1).
- **Preguntas abiertas** (Debilidades/Amenazas y opcionales Fortalezas/Oportunidades).
- Estimación de **role-fit** (PM/Líder, Backend/API, Frontend/UX, Data/ML, QA, DevOps).
- **Recomendaciones de capacitación** por persona y **reportes profundos**.

> Coordinadora: **Lizzy Pamela Mejía** — `lpmejiam@unah.hn`  
> Fecha de este paquete: 07/Oct/2025

---

##  Estructura

```
/
├─ FODA_Liderazgo_Analisis.ipynb     # Notebook principal
├─ foda_output.zip                    # Resultados (CSV, PNG, reportes)

```
---

##  Inicio rápido (Colab)

1. Carga `FODA_Liderazgo_Analisis.ipynb` en **Google Colab**.
2. Ejecuta la **Celda 1 (Carga)** y **Celda 2 (Análisis)** (sube `respuestas.xlsx` o usa Drive/URL).
3. Revisa `/content/foda_output/` con CSV y gráficos.
4. (Opcional) Ejecuta celdas 3–7 para diagramas por persona, TF-IDF, clustering, correlaciones y reportes profundos.

---

##  Metodología (resumen)

- Normalización 1–5 → 0–1: `(x-1)/4`.
- Promedios por grupo de competencias (regex configurables).
- Role-fit: suma ponderada por rol / suma de pesos.
- Recomendaciones: brechas numéricas (<0.5) + keywords en abiertas.
- FODA por persona: F/D (cerradas + abiertas), O/A (abiertas/inferencia).

---

##  Troubleshooting

- En Colab usa rutas bajo `/content` (no `/mnt/data`).
- Ajusta regex de `MAP`/`LIKERT_GROUPS` si cambiaste textos.
- Verifica que haya respuestas numéricas para gráficos.

---

##  Contacto

- Emails: `lpmejiam@unah.hn` `02lizzymejia12@gmail.com`
