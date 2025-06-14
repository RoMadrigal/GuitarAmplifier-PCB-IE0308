# GuitarAmplifier-PCB-IE0308

Repositorio para el proyecto final del curso IE0308 sobre el diseño de una PCB de un amplificador para guitarra. Contiene el circuito esquemático, el diseño de la PCB en *KiCad* y documentación sobre los componentes a utilizar, el procedimiento de diseño y otros detalles. 

Este repositorio y sus contenidos fueron diseñados durante el curso IE0308 durante el periodo I-2025 por los siguientes integrantes del equipo:

<div align="center">

|        **Integrantes**      | **Carné** | **Correo electrónico**|
|:---------------------------:|:---------:|:---------------------:|
|    Anthony Calvo García     |   C11433  |  |
|   Rodrigo Madrigal Montes   |   C24458  | rmadrigalmontes@gmail.com |

</div>

## Organización y contenido de los directorios 

Este repositorio contiene dos directorios principales, cuyos contenidos son:

- `kicad_project`: Contiene los archivos del esquemático, PCB y la configuarción del proyecto
    - `CargadorWalkieTalkie.kicad_pcb`
    - `CargadorWalkieTalkie.kicad_pro`
    - `CargadorWalkieTalkie.kicad_sch`

- `outputs`: Contiene todos los archivos de salida de *KiCad*

Si se desea utilizar este diseño y manufacturarlo por medio de un fabricante se deben comprimir los archivos incluidos en la carpeta `outputs` en un archivo `.zip` y este se puede cargar en la página del fabricante para ordenar la fabricación de la PCB.

## Circuito base

El circuito completo del que partimos para diseñar la PCB fue primeramente fue armado y simulado en el simulador *Tina-TI*:

<div align="center">

| ![Circuto completo del diseño*](images/CircuitoFinal2.JPG) |
|:--:|
| *Circuto completo del diseño* |

</div>

> [!NOTE]
> La documentación detallada de funcionamiento de cada etapa del circuito, elección de componentes, y consideraciones de diseño está disponible en la documentación adicional asociada al proyecto (ver `Wiki` de este repostitorio).

## Diseño de la PCB

