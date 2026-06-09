# Bitácora — Técnicas y Herramientas

---

### 5 de marzo de 2026

Tomamos fotografías a la Luna durante el atardecer. Jugamos con los parámetros de la cámara (exposición, apertura, ISO) para ver cómo afectaban el resultado.

---

### 1 de abril de 2026

Revisamos los metadatos EXIF de las fotos de la Luna que habíamos sacado. Con eso pudimos ver exactamente con qué configuración se había tomado cada imagen.

---

### 8 de abril de 2026

El profe explicó cómo funcionan las antenas y mostró varios modelos: dipolo, Moxon, Yagi, paraguas, etc. También empezamos a usar **MMANA-GAL** para simularlas y ver cómo se comportan.

---

### 15 de abril de 2026

Usamos el **RTLSDR** para recibir señales de radio por primera vez. También vimos el tema de batido de ondas, que es básicamente cómo el SDR baja frecuencias altas a rangos que puede procesar la compu. El profe pasó unos scripts en R para analizarlo.

Se definieron algunas cosas del sistema mecánico: montura ecuatorial, transmisión por correas y tensión máxima de 5V para no quemar el Arduino.

---

### 22 de abril de 2026

Cambiamos de SDR# a **SDR++** porque SDR# tenía problemas en Windows. Simulamos en MMANA-GAL distintas antenas para 144,400 MHz:

| Antena           | Ganancia |
|------------------|----------|
| Yagi 3 elementos | 7,83 dBd |
| Moxon            | 5,43 dBd |

La Yagi ganaba en papel, pero la Moxon se veía mejor para integrar al soporte motorizado.

---

### 29 de abril de 2026

Decidimos construir la **Moxon**. La Yagi tenía más ganancia pero la Moxon es más compacta y fácil de montar en el sistema de seguimiento.

Calculamos las dimensiones para 145 MHz con conductor de 1 mm:

| Parámetro             | Valor      |
|-----------------------|------------|
| Ancho (A)             | 748,8 mm   |
| Excitador (B)         | 108,0 mm   |
| Separación (C)        | 25,8 mm    |
| Long. excitador       | 964,7 mm   |
| Long. reflector       | 1031,9 mm  |
| Profundidad total     | 275,4 mm   |

También practicamos soldadura con cautín.

---

### 6 de mayo de 2026

No hubo clases por viento Zonda. El profe mandó videos y bibliografía sobre la Moxon para avanzar desde casa.

---

### 13 de mayo de 2026

Armamos la antena: cortamos los tubos y cables con las medidas calculadas y soldamos todo. Hicimos una prueba rápida con walkie-talkie.

El profe mencionó que deberíamos aprovechar mejor el tiempo y trabajar también fuera del horario de clases.

---

### 3 de junio de 2026

Probamos la antena con **SDR++** y buscamos los horarios de paso y frecuencias de la **ISS** y el **Tiangong**. Preparamos todo para intentar recibirlos al día siguiente a las 6am. Por el Tiangong esperábamos escuchar comunicaciones en chino o inglés-chino; por la ISS, señales del norte argentino, Uruguay/Brasil y después España/Francia.

---

### 4 de junio de 2026

Calibramos la antena para verificar que la frecuencia de resonancia e impedancia reales coincidan con lo calculado.
