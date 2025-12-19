# QualitySense-RD15-SIC-ProyectoHackathon




### pip install -r requirements.txt

# 🥑 QualitySense

## Descripción del Proyecto

**QualitySense** es un sistema basado en **visión por computadora e inteligencia artificial** diseñado para **automatizar la detección, clasificación y conteo de aguacates** en líneas de producción agroindustrial.

El aguacate es uno de los productos agrícolas más importantes de la **República Dominicana**, representando cerca del **12.63% de la producción agrícola** y aproximadamente **10.23% de las exportaciones agrícolas**. Sin embargo, su clasificación aún se realiza mayormente de forma **manual**, lo que provoca lentitud, errores y mayores costos.

---

## Problemática

* Clasificación manual dependiente del ojo humano.
* Hasta **20% de error** en la separación por tamaños.
* Procesos lentos y poco escalables.
* Incremento de costos operativos.

---

## Objetivo

Desarrollar un sistema inteligente capaz de **detectar, clasificar y contar aguacates en tiempo real**, aumentando la eficiencia del proceso y reduciendo errores humanos.

---

## Enfoque Técnico

El proyecto utiliza **YOLO (You Only Look Once)** con **transfer learning** para detección de objetos.

* 📸 Dataset: Más de **3,500 imágenes** de aguacates etiquetadas.
* 🎯 Precisión: Superior al **90%**.
* ⚡ Mejora de velocidad: Aproximadamente **40%**.

---

## Tecnologías Utilizadas

* Python
* Ultralytics YOLO
* OpenCV
* Streamlit
* SQLite
* spaCy
* Matplotlib & Seaborn

---

## Entrenamiento del Modelo

* Modelo inicial: `yolo11s.pt` (mAP50-95: 0.556)
* Modelo final: `yolo11m.pt` (mAP50-95: 0.572)

El modelo final se guarda como:

```
best.pt
```

---

## Ejecución e Inferencia

Instalar dependencias:

```bash
pip install ultralytics streamlit opencv-python spacy matplotlib seaborn
```

Ejecutar inferencia:

```bash
yolo detect predict model=best.pt source=imagen.jpg
```

---

## Módulo de Visualización

El sistema incluye una **interfaz web en Streamlit** que permite:

* Visualizar estadísticas de producción.
* Consultar datos por tamaño y calidad.
* Realizar consultas en lenguaje natural mediante un **chatbot con NLP**.

Los datos se almacenan en una base de datos **SQLite** para análisis histórico.

---

## Impacto y Escalabilidad

* Reducción de errores y costos operativos.
* Disminución de costos de implementación hasta en **50%**.
* Diseño **escalable**, adaptable a otros productos agrícolas o industriales.

---

## Conclusión

QualitySense demuestra cómo la **inteligencia artificial aplicada** puede modernizar la agroindustria, haciendo los procesos más eficientes, precisos y accesibles.

> *Automatizar hoy es producir mejor mañana.*
