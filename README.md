# Laboratorio 03 - Tecnología Inalámbrica

## Efectos de Propagación a Gran Escala

**Integrantes:**

- Felipe Bustos López
- Francisco Polanco Alfaro

---

## Descripción

En este laboratorio se evaluó experimentalmente la pérdida de potencia de una señal de **2,67 GHz** al variar la distancia entre el transmisor y el receptor.

Para realizar las mediciones se utilizó un generador de señales como transmisor y un analizador de espectro como receptor. La señal fue medida a distintas distancias, manteniendo constantes la frecuencia, la potencia transmitida, la altura y la polarización de las antenas.

Los resultados experimentales fueron utilizados para caracterizar el modelo de propagación **log-distance con ensombrecimiento log-normal**, obteniendo el exponente de pérdida de trayecto, la desviación estándar del ensombrecimiento y el coeficiente de determinación del ajuste.

---

## Equipamiento utilizado

- Generador de señales **Rohde & Schwarz SMC100A**.
- Analizador de espectro **Rohde & Schwarz FSH4**.
- 2 antenas omnidireccionales **Multiband Rubber Duck - Pasternack**, con ganancia de 4,5 dBi.
- Alargador eléctrico de 20 m.
- 2 conectores N-SMA.
- Computador para el registro y procesamiento de los datos.

---

## Condiciones de medición

La experiencia se realizó en el pasillo del nivel 4 de Ejército.

Los principales parámetros utilizados fueron:

| Parámetro | Valor |
|---|---:|
| Frecuencia de operación | 2670 MHz |
| Potencia transmitida | 0 dBm |
| Ganancia antena transmisora | 4,5 dBi |
| Ganancia antena receptora | 4,5 dBi |
| Distancia inicial | 1 m |
| Distancia final | 15 m |
| Número de mediciones | 42 |
| Distancia de referencia | 1 m |
| Longitud de onda aproximada | 11,2 cm |

Entre 1 m y 3,9 m se realizaron mediciones cada 10 cm. Desde 4 m hasta 15 m se realizaron mediciones cada 1 m.

---

## Resultados principales

A partir de las mediciones obtenidas se determinaron los siguientes parámetros para el modelo de propagación:

| Parámetro | Valor | Unidad |
|---|---:|---|
| Exponente de pérdida `n` | 2,30 | - |
| Pérdida de referencia `PL(d0)` | 57,80 | dB |
| Desviación estándar `σ` | 1,92 | dB |
| Coeficiente de determinación `R²` | 0,937 | - |
| Número de muestras `N` | 42 | - |
| Pérdida en espacio libre a `d0` | 40,98 | dB |
| Exceso sobre espacio libre | 16,82 | dB |
| Potencia ajustada en `d0` | -48,80 | dBm |
| Distancia de campo lejano `df` | 0,26 | m |

La potencia recibida disminuyó desde **-46,3 dBm a 1 m** hasta **-75,3 dBm a 15 m**, correspondiente a una disminución de **29,0 dB**.

El ajuste obtenido presentó un `R² = 0,937`, lo que indica que la distancia explica una parte importante de la variación observada en la potencia recibida.

---

## Evidencia experimental

La carpeta `Evidencia/` contiene las fotografías obtenidas durante la experiencia.

Las imágenes corresponden a los registros realizados con el analizador de espectro y a las diferentes posiciones del montaje experimental.

La evidencia permite respaldar las mediciones utilizadas posteriormente para calcular la pérdida de trayecto y obtener los parámetros del modelo.

---

## Archivo de datos

El archivo Excel contiene las mediciones experimentales y el procesamiento utilizado para obtener los resultados:

`Excel/Lab3_Propagacion_Gran_Escala.xlsx`

Este archivo permite revisar los valores de potencia registrados, los cálculos realizados y los resultados utilizados para el análisis del modelo.

---

## Informe

El informe completo del laboratorio se encuentra en:

`Informe/Lab3_TI_Final.pdf`

El documento contiene:

- Resumen.
- Introducción.
- Marco teórico.
- Generador de señales.
- Analizador de espectro.
- Modelo de ensombrecimiento log-normal.
- Metodología.
- Equipamiento utilizado.
- Montaje experimental.
- Procedimiento de medición y procesamiento de datos.
- Resultados y discusión.
- Mediciones de potencia recibida.
- Parámetros del modelo.
- Campo lejano y comparación con espacio libre.
- Registro del analizador.
- Comparación con la literatura.
- Conceptos demostrados.
- Dificultades y aspectos relevantes de la experiencia.
- Aplicaciones posibles.
- Evidencia de las mediciones.
- Conclusiones.
- Referencias.

---

## Organización del repositorio

La estructura del laboratorio es la siguiente:

```text
LAB03/
│
├── README.md
│
├── Excel/
│   └── Lab3_Propagacion_Gran_Escala.xlsx
│
├── Evidencia/
│   ├── 1.1.jpeg
│   ├── 1.2.jpeg
│   ├── 1.3.jpeg
│   ├── 1.4.jpeg
│   ├── 1.5.jpeg
│   ├── 1.6.jpeg
│   ├── 1.7.jpeg
│   ├── 1.8.jpeg
│   ├── 1.9.jpeg
│   ├── 2.jpeg
│   ├── 2.1.jpeg
│   ├── 2.2.jpeg
│   ├── 2.3.jpeg
│   ├── 2.4.jpeg
│   ├── 2.5.jpeg
│   ├── 2.6.jpeg
│   ├── 2.7.jpeg
│   ├── 2.8.jpeg
│   ├── 2.9.jpeg
│   ├── 3.jpeg
│   ├── 3.1.jpeg
│   ├── 3.2.jpeg
│   ├── 3.3.jpeg
│   ├── 3.4.jpeg
│   ├── 3.5.jpeg
│   ├── 3.6.jpeg
│   ├── 3.7.jpeg
│   ├── 3.8.jpeg
│   ├── 3.9.jpeg
│   ├── 4.jpeg
│   ├── 5.jpeg
│   ├── 6.jpeg
│   ├── 7.jpeg
│   ├── 8.jpeg
│   ├── 9.jpeg
│   ├── 10.jpeg
│   ├── 11m.jpeg
│   ├── 12.jpeg
│   ├── 13.jpeg
│   ├── 14.jpeg
│   ├── 15.jpeg
│   └── captura 1 metro.jpg
│
└── Informe/
    └── Lab3_TI_Final.pdf
```

---

## Repositorio

El informe, los datos utilizados para el procesamiento y las evidencias experimentales se encuentran disponibles en el repositorio de GitHub:

**Repositorio de GitHub:**  
https://github.com/sephppx/Laboratorio-03---Tecnologia-Inalambrica

---

## Autores

**Felipe Bustos López**  
**Francisco Polanco Alfaro**

**Tecnología Inalámbrica, 2026**
