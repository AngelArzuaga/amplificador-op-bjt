# Amplificador Operacional con BJTs

Diseño de un amplificador operacional discreto construido con transistores BJT, incluyendo esquemático, simulación en LTspice y layout en KiCad.

## Descripción

<!-- Reemplaza esto con una descripción breve: qué topología usa (par diferencial, push-pull, etc.), 
     para qué está pensado, y qué lo hace interesante de tu diseño. -->

Este proyecto implementa un amplificador operacional de propósito general utilizando transistores bipolares discretos, sin depender de un CI integrado. El objetivo es [explorar el diseño analógico a nivel de transistor / cumplir con una práctica académica / etc.].

## Especificaciones

| Parámetro | Valor |
|---|---|
| Ganancia en lazo abierto | XX dB |
| Ancho de banda | XX kHz |
| Voltaje de alimentación | ±XX V |
| Impedancia de entrada | XX kΩ |
| Impedancia de salida | XX Ω |
| Slew rate | XX V/µs |

## Estructura del repositorio

```
amplificador-op-bjt/
├── kicad/          # Esquemático y PCB (KiCad)
├── ltspice/         # Simulaciones y resultados (LTspice)
├── datasheets/       # Hojas de datos de los componentes usados
├── docs/
│   └── images/         # Capturas de esquemático, gráficas, fotos
├── gerbers/           # Archivos de fabricación del PCB
└── LICENSE
```

## Esquemático

![Esquemático](docs/images/esquematico.png)

## Simulación en LTspice

<!-- Agrega aquí una imagen de la respuesta en frecuencia, transitoria, etc. -->

![Resultados de simulación](docs/images/simulacion.png)

*Breve descripción de qué muestra la simulación: por ejemplo, respuesta en frecuencia con ganancia de XX dB y ancho de banda de XX kHz.*

## PCB

![PCB](docs/images/pcb.png)

## Componentes utilizados

| Componente | Valor / Modelo | Datasheet |
|---|---|---|
| Q1, Q2 | 2N3904 | [datasheet](datasheets/2N3904.pdf) |
| Q3 | 2N3906 | [datasheet](datasheets/2N3906.pdf) |
| R1 | 10 kΩ | — |
| C1 | 100 nF | — |

## Cómo abrir los archivos

**KiCad** (versión 9.0 o superior):
1. Abre KiCad
2. File → Open Project → selecciona `kicad/amp-op-bjt.kicad_pro`

**LTspice**:
1. Abre LTspice
2. File → Open → selecciona el archivo `.asc` dentro de `ltspice/`
3. Ejecuta la simulación con Simulate → Run

## Licencia

Este proyecto está licenciado bajo **CERN-OHL-P v2**. Ver [LICENSE](LICENSE) para el texto completo.
