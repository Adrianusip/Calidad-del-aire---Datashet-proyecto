# Calidad del aire - Dataset de humo

En este proyecto creamos un dataset con imágenes de humo para utilizarlo junto con nuestro proyecto de calidad del aire. Recopilamos y organizamos las imágenes para posteriormente entrenar un modelo que pueda identificar la presencia de humo y apoyar en la detección de contaminación.

## Dataset

El dataset contiene 100 imágenes relacionadas con humo.

Las imágenes originales se encuentran en:

datos/
└── raw/
    ├── humo_001.jpg
    ├── humo_002.jpg
    ├── ...
    └── humo_100.jpg

También se cuenta con una versión organizada para YOLO:

dataset_yolo/
├── images/
│   ├── train/
│   └── val/
├── labels/
│   ├── train/
│   └── val/
└── data.yaml

## Organización

Las 100 imágenes fueron divididas en:

- 80 imágenes para entrenamiento.
- 20 imágenes para validación.

Cada imagen del dataset YOLO cuenta con su archivo de etiquetas correspondiente.

## Scripts

La carpeta scripts/ contiene herramientas utilizadas para trabajar con el dataset:

scripts/
├── descargar_pesos_sam3.py
└── sam3_recortar_dataset.py

## Objetivo

El objetivo del dataset es utilizar las imágenes de humo para entrenar un modelo de visión artificial que pueda reconocer humo y posteriormente integrarlo como apoyo en nuestro proyecto de calidad del aire.

## Tecnologías

- Python
- YOLO
- SAM 3
- Git y GitHub