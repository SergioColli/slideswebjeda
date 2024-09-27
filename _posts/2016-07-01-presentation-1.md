---
title: "Unidad 2: Actuadores"
layout: post
permalink: /unidad-2-actuadores/
background: '#0a5'

slides:
  - title: "Unidad 2: Actuadores"
    slide-data: |
      Los actuadores convierten energía en movimiento. Se clasifican principalmente en tres tipos:
      - Eléctricos
      - Mecánicos
      - Hidráulicos
    background: '#3498db'

  - title: "2.1 Eléctricos"
    slide-data: "Los actuadores eléctricos utilizan energía eléctrica para generar movimiento."

  - title: "2.1.1 Tipos"
    slide-data: |
      - Motores DC
      - Motores paso a paso
      - Servomotores

  - title: "2.1.2 Funcionamiento"
    slide-data: "Convierte la energía eléctrica en energía mecánica."

  - title: "2.1.3 Características"
    slide-data: |
      - Alta precisión
      - Control sobre velocidad y posición

  - title: "2.1.4 Modo de comunicación"
    slide-data: |
      - PWM (Modulación por Ancho de Pulso)
      - Comunicación serial

  - title: "2.2 Mecánicos"
    slide-data: "Los actuadores mecánicos generan movimiento a partir de componentes mecánicos."

  - title: "2.2.1 Tipos"
    slide-data: |
      - Engranajes
      - Resortes
      - Poleas

  - title: "2.2.2 Funcionamiento"
    slide-data: "El movimiento se genera mediante la interacción mecánica entre componentes."

  - title: "2.2.3 Características"
    slide-data: |
      - Generalmente económicos
      - Fiabilidad en aplicaciones simples

  - title: "2.2.4 Modo de comunicación"
    slide-data: "Movimientos manuales o automatizados por mecanismos eléctricos."

  - title: "2.3 Hidráulicos"
    slide-data: "Los actuadores hidráulicos emplean fluidos bajo presión para generar movimiento."

  - title: "2.3.1 Tipos"
    slide-data: |
      - Cilindros hidráulicos
      - Motores hidráulicos

  - title: "2.3.2 Funcionamiento"
    slide-data: "Se utiliza la presión de un fluido para mover un pistón o generar torque."

  - title: "2.3.3 Características"
    slide-data: |
      - Fuerza muy alta
      - Precisión baja en comparación con otros actuadores

  - title: "2.3.4 Modo de comunicación"
    slide-data: |
      - Válvulas y controladores de flujo

  - title: "Fin de la Presentación"
    slide-data: "¡Gracias!"
---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
  <h1>{{slide.title}}</h1>
  <p>{{ slide.slide-data | markdownify }}</p>
</section>               
{% endfor %}
