# GuitarAmplifier-PCB-IE0308

Repositorio para el proyecto final del curso IE0308 sobre el diseño de una PCB de un amplificador para guitarra. Contiene el circuito esquemático, el diseño de la PCB en *KiCad* y documentación sobre los componentes a utilizar, el procedimiento de diseño y otros detalles. 

Este repositorio y sus contenidos fueron diseñados durante el curso IE0308 durante el periodo I-2025 por los siguientes integrantes del equipo:

<div align="center">

|        **Integrantes**      | **Carné** | **Correo electrónico**|
|:---------------------------:|:---------:|:---------------------:|
|    Anthony Calvo García     |   C11433  |  anthonycalvo50@gmail.com |
|   Rodrigo Madrigal Montes   |   C24458  | rmadrigalmontes@gmail.com |

</div>

## Agradecimientos a PCBWay

Queremos expresar nuestro agradecimiento a **PCBWay** por su colaboración y apoyo en la fabricación de nuestras PCBs. La calidad de las placas recibidas, tanto en precisión de fabricación como en acabados, fue sobresaliente. Todo el proceso desde la carga de archivos hasta la recepción del paquete fue ágil, transparente y eficiente. 

Además siempre estuvieron disponibles para cualquier consulta, para asegurarse de que todo saliera según lo planeado, lo cual nos brindó mucho soporte y seguridad durante todo el proceso de pedido.

### PCB ensamblada

Una vez recibidas las placas de **PCBWay**, se procedió con el ensamblaje manual de todos los componentes. A continuación se muestran imágenes del resultado final:

<div align="center">

| ![PCB ensamblada - sin los componentes externos conectados](images/PCB_Alone.jpg) |
|:--:|
| *PCB ensamblada - sin los componentes externos conectados* |

</div>

<div align="center">

| ![PCB ensamblada - con los componentes externos conectados](images/PCB_Build.jpg) |
|:--:|
| *PCB ensamblada - con los componentes externos conectados* |

</div>

### Demostración de funcionamiento

A continuación, se presentan vídeos demostrativos del amplificador montado, funcionando correctamente tanto con una guitarra eléctrica como con un teléfono:

<p align="center">
  <a href="https://youtu.be/fU8gYd2I1fY" target="_blank">
    <img src="images/GuiVid.png" alt="Demo con guitarra eléctrica" width="480"/>
  </a>
  <br/>
  <em>Demostración del amplificador conectado a una guitarra eléctrica</em>
</p>

<p align="center">
  <a href="https://youtu.be/jr76lwe1I88" target="_blank">
    <img src="images/SmPVid.png" alt="Demo con teléfono móvil" width="480"/>
  </a>
  <br/>
  <em>Demostración del amplificador reproduciendo audio desde un teléfono</em>
</p>

Gracias a su servicio confiable y de altísima calidad, logramos ensamblar y probar con éxito nuestro amplificador, cumpliendo los objetivos del proyecto. Recomendamos sus servicios para estudiantes, profesionales y cualquier persona interesada en manufacturar PCBs de alta calidad. Más información en [pcbway.com](https://www.pcbway.com).

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

### Lista de componentes

A continuación se incluye una lista con los componentes utilizados en el diseño, con el mismo número que se les asignó en el diseño final de PCB:

<div align="center">

|   Componente   |   Valor / Modelo    |    Descripción    |
|:--------------:|:-------------------:|:-----------------:|
| R1 / R2   |     1 kΩ           |   Resistor de película metálica    |
| R3    |     1 MΩ           |   Resistor de película metálica     |
| R4    |     100 Ω           |   Resistor de película metálica     |
| R5    |     10 kΩ           |   Resistor de película metálica     |
| R6    |     3 kΩ           |   Resistor de película metálica     |
| R7 / R8    |     1.5 kΩ     |   Resistor de película metálica     |
| R9    |     3.3 kΩ           |   Resistor de película metálica     |
| R10    |     33 kΩ           |   Resistor de película metálica     |
| R11    |     170 Ω           |   Resistor de película metálica     |
| R12    |     10 Ω           |   Resistor de película metálica     |
| C1 / C3 / C11 / C15    |     470 nF          | Capacitor cerámico |
| C2 / C6 / C7 / C12   |     100 nF          | Capacitor de poliéster |
| C4 / C5 / C8 / C10 / C16   |     220 nF          | Capacitor de poliéster |
| C9    |     10 nF          | Capacitor de poliéster |
| C13    |     10 μF          | Capacitor electrolítico |
| C14    |     220 μF          | Capacitor electrolítico |
| U1 / U2   |     TL072CP      | Amplificador operacional |
| U3    |     LM386            | Amplificador de potencia |
| D1    |     1N4148            | Diodo rectificador |
| Gain / Low / Mid / High    |     50 kΩ            | Potenciómetro logarítmico |
| Volume    |     10 kΩ            | Potenciómetro logarítmico |
| J1    |     -         | Jack estéreo 6,3 mm |
| Battery / Speaker    |     -         | Terminal 01x02 5.08mm |
| Clean / O.D. Switch    |     -         | Terminal 01x03 5.08mm |

</div>

## Diseño de la PCB

Una vez definido el circuito final, se diseñó la PCB en *KiCad* con una arquitectura de **cuatro capas**:

- **F.Cu**: Ruta de señales
- **In1.Cu**: Plano de alimentación (+9V y +4.5V)
- **In2.Cu**: Plano de tierra (GND)
- **B.Cu**: Ruta de señales

### Capas de la PCB

<div align="center">

| ![Capa F.Cu](images/F.Cu.png) |
|:-----------------------------:|
|    *Capa superior (F.Cu)*     |

</div>

<div align="center">

| ![Capa B.Cu](images/B.Cu.png) |
|:-----------------------------:|
|    *Capa inferior (B.Cu)*     |

</div>

<div align="center">

| ![In1.Cu - Alimentación](images/In1.Cu.png) |
|:-------------------------------------------:|
|      *Capa interna 1 - +9V / +4.5V*         |

</div>

<div align="center">

| ![In2.Cu - Tierra](images/In2.Cu.png) |
|:-------------------------------------:|
|        *Capa interna 2 - GND*         |

</div>

Además, se agregaron zonas de serigrafía, agujeros de montaje, así como textos identificativos y logotipos en el *silkscreen* con el nombre del proyecto y los autores.

<div align="center">

| ![Vista 3D de la PCB](images/Vista3DSuperior.png) |
|:--:|
| *Vista 3D de la PCB en KiCad* |

</div>