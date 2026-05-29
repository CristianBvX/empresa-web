# Guía Completa de Configuración y Ajuste de Frecuencias
## Sistema de Audio Profesional a 3 Vías Mono (Operación a 8 Ohms)

Esta guía técnica detalla la calibración precisa, el ruteo de señal y los puntos de corte óptimos para el sistema de audio, garantizando el máximo impacto acústico (patada en el pecho), un bajo profundo y controlado, y protección absoluta de todos los componentes contra fallas mecánicas o térmicas.

---

## 1. Esquema de Componentes y Potencia (Carga a 8 Ω)

El sistema está diseñado para trabajar con una sola bocina por canal, lo que representa la configuración más segura, lineal y eficiente para los amplificadores, minimizando el calentamiento y la distorsión.

| Vía Acústica | Componentes Físicos | Amplificador Asignado | Potencia Real de Trabajo (RMS) |
| :--- | :--- | :--- | :--- |
| **Baja (Sub-Graves)** | 2 x Cajones con bocinas **Krack KPA-18B (18")** | **Backstage HCF Pro 40** | Alta corriente / Alto Factor de Amortiguamiento |
| **Media (Medios-Bajos)** | 2 x Cajones con bocinas **B-52 15-85 (15")** | **Backstage CS 20000** | **310W RMS** por canal a 8 Ohms |
| **Alta (Medios-Agudos)** | Torres superiores con **Crossover Pasivo Radox 600W** | **Backstage CS 16000** | **290W RMS** por canal a 8 Ohms |

---

## 2. Configuración Física del Crossover (Panel Trasero)

Para habilitar las tres salidas independientes desde el rack, el crossover **Backstage BS-183** debe trabajar en modo unificado.

1. **Selector de Modo (MODE):** Presionar el botón cuadrado trasero para activar el modo **MONO**. 
2. **Ruteo de Cables (Guiarse estrictamente por el texto inferior de la serigrafía):**
   * **INPUT:** Conectar el cable de señal principal proveniente de la mezcladora (Canal Maestro / Mono).
   * **LOW OUT:** Conectar a la entrada del amplificador **HCF Pro 40** (Sub-graves).
   * **MID OUT:** Conectar a la entrada del amplificador **CS 20000** (Medios-Bajos).
   * **HIGH OUT:** Conectar a la entrada del amplificador **CS 16000** (Medios-Agudos).
   * *Nota: Los conectores centrales marcados en el modo estéreo quedan inactivos en esta modalidad.*

---

## 3. Calibración y Cortes de Frecuencia (Panel Frontal)

*Al estar en modo Mono, el control de todo el sistema se realiza exclusivamente con las perillas del panel frontal leyendo las etiquetas impresas en color **ROJO** en la parte inferior.*

```
   [ FREQ LOW/MID ]                  [ FREQ MID/HIGH ] (x10 Presionado)
      110Hz - 120Hz                             250 (2,500 Hz)
          │                                         │
 ◄────────┴────────►                       ◄────────┴────────►
   GRAVES (Krack 18")                       MEDIOS (B-52 15")     AGUDOS (Brillo)
   (Hasta 110-120 Hz)                      (110 Hz a 2,500 Hz)   (De 2,500 Hz en adelante)
```

### A. Perilla LOW/MID (Corte de Sub-Graves a Medios-Bajos)
* **Ajuste Físico:** Colocar la perilla apuntando entre los **110 Hz y 120 Hz**.
* **Multiplicador (Botón x10):** Debe estar **AFUERA** (desactivado).
* **Propósito Técnico:** * Establece el límite superior de los subwoofers Krack. Al frenar la señal antes de los 140 Hz, se elimina de raíz el "aporreo" mecánico del cono contra el fondo del imán y las resonancias parásitas de la madera, manteniendo un bajo sumamente firme y profundo.
  * Define el inicio de la respuesta para las bocinas B-52 de 15 pulgadas.

### B. Perilla MID/HIGH (Corte de Medios-Bajos a Agudos Puros)
* **Ajuste Físico:** Colocar la perilla apuntando exactamente al número **250**.
* **Multiplicador (Botón x10):** Debe estar **PRESIONADO** (activado). Al activarse, el valor de la perilla se multiplica por 10, ejecutando un corte real en los **2,500 Hz**.
* **Propósito Técnico:** * Encierra el rango de trabajo de las B-52 en su zona de máximo rendimiento (110 Hz a 2,500 Hz), permitiéndoles concentrar toda la energía del amplificador en la "patada" seca del bombo, las congas y el cuerpo de las voces tropicales, sin gastar energía en sub-graves lentos ni en brillos altos.
  * Envía de los 2,500 Hz hacia arriba de manera limpia a las cajas superiores.

### C. Ajuste de Fase (Botón INV)
* **Configuración:** El botón **INV** (Inversión de polaridad) para la vía de graves debe permanecer **AFUERA** (Desactivado).
* **Física Acústica:** Las pruebas auditivas confirman que la polaridad original es la correcta. Mantener el botón desactivado asegura que los conos empujen el aire hacia el frente de manera unísona, evitando cancelaciones de fase en la pista y previniendo que el sonido se "aleje" o se escuche hueco.

---

## 4. Gestión de Ganancias y Protocolo de Protección

### Vía Alta (Medios-Agudos - Placa Radox 600W)
La placa pasiva Radox tiene un umbral máximo de resistencia térmica de 600W continuos y **carece de sistemas de protección sacrificables** (no tiene focos de halógeno ni fusibles de cristal). 

A pesar de que el amplificador CS 16000 entrega **290W RMS a 8 Ohms** (lo cual se encuentra perfectamente dentro del rango seguro y garantiza un *headroom* libre de distorsión), un exceso de volumen sostenido desde la mezcladora puede sobrecalentar las resistencias cerámicas blancas de la placa.
* **Acción obligatoria:** No abrir las ganancias físicas del amplificador CS 16000 a más del **50% o 60%**. Es técnicamente superior mantener el amplificador trabajando relajado y nivelar la presencia del brillo en la pista de baile utilizando exclusivamente la perilla **GAIN HIGH OUT** del crossover frontal.

### Vía Media (Medios-Bajos - B-52 15")
El amplificador CS 20000 entrega **310W RMS a 8 Ohms**. Este nivel de potencia es idóneo para que la suspensión de las bocinas de 15" reaccione con velocidad extrema ante los remates de percusión. Puede operarse con amplitud, vigilando que los indicadores de *CLIP* en el amplificador nunca se enciendan de forma fija.

### Acomodo Físico en Eventos (La Torre Perfecta)
Para maximizar el rendimiento de las frecuencias y evitar pérdidas de presión acústica en espacios abiertos:
1. **Base (Piso):** Ambos subwoofers de 18" deben colocarse juntos o apilados al centro o en un solo costado. El acoplamiento físico duplica el impacto frontal en la pista.
2. **Cuerpo (En medio):** Las cajas B-52 de 15" van inmediatamente arriba de los bajos para dar una continuidad natural al golpe medio-bajo. *(Se recomienda usar soportes de goma o cintas tensoras para evitar que caminen por la vibración).*
3. **Corona (Hasta arriba):** Las cajas de medios-agudos deben estar en la cima, elevadas por encima de la altura de la cabeza del público, permitiendo que las frecuencias altas (que viajan en línea recta como un haz de luz) proyecten la voz del animador a larga distancia sin ser bloqueadas por los cuerpos de los bailarines.
