# Proyecto A/B Test – Sistema de Recomendaciones

## Contexto
Has recibido la tarea analítica de una tienda en línea internacional.  
Los predecesores iniciaron un **test A/B** para evaluar un nuevo embudo de pago y un sistema de recomendaciones mejorado, pero no completaron el análisis. Solo dejaron las especificaciones técnicas y los resultados de la prueba.  

El objetivo de este proyecto es **verificar si la prueba se realizó correctamente**, analizar los resultados y generar insights para optimizar la conversión de usuarios en el embudo de ventas: `product_page → product_card → purchase`.

---

## Descripción Técnica

- **Nombre de la prueba:** `recommender_system_test`  
- **Grupos:** A (control), B (nuevo embudo de pago)  
- **Fechas clave:**  
  - Lanzamiento: 2020-12-07  
  - Fin de aceptación de nuevos usuarios: 2020-12-21  
  - Finalización del test: 2021-01-01  
- **Audiencia:** 15% de los nuevos usuarios de la región de la UE  
- **Propósito:** probar cambios relacionados con un sistema de recomendaciones mejorado  
- **Resultado esperado:** al menos un 10% de aumento en cada etapa del embudo (`product_page → product_card → purchase`) durante los 14 días posteriores a la inscripción  
- **Número previsto de participantes:** 6 000 usuarios

---

## Datos Utilizados

### `ab_project_marketing_events_us.csv`
- `name`: nombre del evento de marketing  
- `regions`: regiones donde se llevará a cabo la campaña  
- `start_dt`: fecha de inicio de la campaña  
- `finish_dt`: fecha de finalización  

### `final_ab_new_users_upd_us.csv`
- `user_id`  
- `first_date`: fecha de inscripción  
- `region`  
- `device`: dispositivo utilizado  

### `final_ab_events_upd_us.csv`
- `user_id`  
- `event_dt`: fecha y hora del evento  
- `event_name`: tipo de evento (`product_page`, `product_card`, `purchase`)  
- `details`: datos adicionales, como el monto de la compra en USD  

### `final_ab_participants_upd_us.csv`
- `user_id`  
- `ab_test`: nombre de la prueba  
- `group`: grupo de prueba (A o B)  

---

## Objetivos del Análisis

1. **Validación de la prueba**  
   - Comprobar que todos los participantes estén correctamente asignados a su grupo  
   - Verificar que la muestra cumpla con el tamaño esperado y la distribución entre grupos  

2. **Análisis del embudo de conversión**  
   - Medir la tasa de eventos `product_page → product_card → purchase` por grupo  
   - Comparar el rendimiento entre grupo A (control) y grupo B (nuevo embudo)  

3. **Detección de posibles sesgos**  
   - Analizar la distribución por región, fecha de inscripción y dispositivo para asegurar que los grupos son comparables  

4. **Cálculo del efecto de la prueba**  
   - Determinar si el nuevo embudo de pago y el sistema de recomendaciones mejorado generaron al menos un **10% de aumento** en cada etapa del embudo  

---

## Valor del Proyecto
Este análisis permite:  
- Evaluar la efectividad de un nuevo sistema de recomendaciones en el comportamiento de los usuarios  
- Detectar mejoras concretas en la conversión de productos  
- Brindar información accionable para futuras campañas de marketing y optimización del embudo de ventas  

---
