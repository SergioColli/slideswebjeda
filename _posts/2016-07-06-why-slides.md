---
title: "Unidad 2: Actuadores"
layout: post
permalink: /unidad-2-actuadores/
background: '#0a5'

slides:
  - title: "Unidad 2: Actuadores"
    slide-data: |
      Los actuadores convierten energía en movimiento.
      Se clasifican principalmente en tres tipos:
      - Eléctricos
      - Mecánicos
      - Hidráulicos

  - title: "2.1 Actuadores Eléctricos"
    slide-data: "Utilizan energía eléctrica para generar movimiento."

  - title: "2.1.1 Tipos de Motores"
    slide-data: |
      - Motores DC
      - Motores paso a paso
      - Servomotores

  - title: "2.1.2 Funcion"
    slide-data: "Convierte energía eléctrica en energía mecánica."

  - title: "2.1.3 Características"
    slide-data: |
      - Alta precisión
      - Control sobre velocidad y posición

  - title: "2.1.4 Comunicación"
    slide-data: |
      - PWM (Modulación por Ancho de Pulso)
      - Comunicación serial

  - title: "2.2 Actuadores Mecánicos"
    slide-data: "Generan movimiento a partir de componentes mecánicos."

  - title: "2.2.1 Tipos de Componentes"
    slide-data: |
      - Engranajes
      - Resortes
      - Poleas

  - title: "2.2.2 Funcionamiento"
    slide-data: "Movimiento generado mediante la interacción mecánica."

  - title: "2.2.3 Características"
    slide-data: |
      - Generalmente económicos
      - Fiabilidad en aplicaciones simples

  - title: "2.2.4 Comunicación"
    slide-data: "Movimientos manuales o automatizados."

  - title: "2.3 Actuadores Hidráulicos"
    slide-data: "Emplean fluidos bajo presión para generar movimiento."

  - title: "2.3.1 Tipos de Hidráulicos"
    slide-data: |
      - Cilindros hidráulicos
      - Motores hidráulicos

  - title: "2.3.2 Funcionamiento"
    slide-data: "Utilizan presión de fluido para mover un pistón."

  - title: "2.3.3 Características"
    slide-data: |
      - Fuerza muy alta
      - Precisión baja comparado con otros actuadores

  - title: "2.3.4 Comunicación"
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
