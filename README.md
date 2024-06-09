# Tarea01Dis

## Descripción
Este proyecto combina el patrón Observer y AspectJ para gestionar cambios de color en la interfaz de una aplicación simple, con botones que cambian el color de fondo de la ventana.

## Funcionalidades
- **Cambio de Color**: Los botones permiten cambiar el color de fondo de la ventana a rojo, verde o azul.
- **Registro en Consola**: Cada cambio se registra en la consola, indicando el nuevo color de fondo.

## Funcionalidad Adicional: Registro de Actividades con AspectJ
- **Propósito de la Funcionalidad AOP**: Implementamos un aspecto específico utilizando AspectJ para separar la lógica de registro de eventos de la lógica de la interfaz de usuario. Esta separación ilustra un principio clave de la Programación Orientada a Aspectos (AOP), que es manejar las preocupaciones transversales de manera independiente del código principal.
- **Implementación**: Un aspecto intercepta los clics en los botones y registra cada evento en un archivo `colorChangeLog.txt`. Esta funcionalidad AOP permite mantener un registro detallado de las interacciones del usuario sin ensuciar la lógica principal del cambio de color.
- **Detalles del Registro**: Cada entrada en `colorChangeLog.txt` documenta el número de clics y el color seleccionado, ofreciendo un histórico exhaustivo de las acciones del usuario que puede usarse para auditorías o análisis de comportamiento.

### Importancia del Aspecto en el Proyecto
El uso de AspectJ para el registro de actividades demuestra cómo los aspectos pueden mejorar la claridad y la organización del código al manejar funcionalidades secundarias de forma automática y desacoplada. Esto no solo simplifica el mantenimiento del código principal, sino que también realza la capacidad de ampliar el proyecto con nuevas características sin alterar su estructura central.

## Conclusión
La integración de AOP en este proyecto subraya la utilidad de AspectJ para abordar eficazmente las preocupaciones transversales, garantizando que la aplicación permanezca robusta, escalable y fácil de mantener.
