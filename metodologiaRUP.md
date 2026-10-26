# Aplicación de la metodología RUP al Sistema de Pedidos con Delivery y Recojo en Local

El proyecto que vamos a desarrollar es el Sistema de Pedidos con Modalidad Delivery y Recojo en Local, propuesto para un restaurante en el documento del IESTP José Pardo.

Aplicaremos la metodología RUP (Rational Unified Process) a este negocio, utilizando sus cuatro fases: Inicio, Elaboración, Construcción y Transición. El objetivo es organizar el desarrollo del sistema para reducir los errores al tomar pedidos por WhatsApp o llamadas telefónicas, mejorar la atención al cliente y controlar las ventas.

## 1. Fase de Inicio

Objetivo: definir el problema, los objetivos y la viabilidad del sistema.

En esta fase se identifica qué necesita el restaurante y qué funcionalidades tendrá el software.

[Caisse enregistreuse fast-food dès 0 €/mois | shopcaisse](https://images.openai.com/static-rsc-4/_Dpz0rSBSGotL1rT6JDJGT-CCDecTg1DKK70WVGwnKuwr5t4PMu3UzwNegdBwomskOQxFYRNJ0DIpH1oe0ZO_B70GUhmORxYAfttf4WsXTy8oUATvmbSCrTZVWtJg9ENHbmPLAbuU-S18OAUDtzRUvLGZfYOkw00qPuMgFoiD7c?purpose=inline)

Problema identificado

Actualmente, los pedidos se pueden registrar manualmente mediante llamadas o WhatsApp, lo que puede ocasionar errores en las cantidades, demoras en la confirmación y dificultades para conocer el estado del pedido.

Requisitos principales

- Mostrar una carta digital con productos, precios y disponibilidad.
- Permitir agregar productos al carrito y personalizar los pedidos.
- Elegir entre delivery y recojo en local.
- Registrar los pagos y generar comprobantes digitales.
- Consultar y actualizar el estado de los pedidos.
- Administrar los productos y revisar indicadores básicos de ventas.

Actores del sistema

| Actor                       | Función                                                  |
| --------------------------- | -------------------------------------------------------- |
| Cliente                     | Consulta la carta, realiza pedidos y revisa su estado.   |
| Personal de atención        | Recibe pedidos y actualiza su estado.                    |
| Administrador               | Gestiona los productos y consulta reportes.              |
| Repartidor                  | Realiza las entregas a domicilio.                        |
| Servicio de geolocalización | Ayuda a verificar la ubicación y cobertura del delivery. |

Resultado de la fase: se define el alcance inicial del proyecto y se determina que la solución propuesta responde a las necesidades del restaurante.

## 2. Fase de Elaboración

Objetivo: analizar los requisitos detalladamente y diseñar la arquitectura del sistema.

Aquí se define cómo funcionará el sistema antes de implementar todas sus funcionalidades.

[Free AI UML Diagram Maker: Create UML Diagrams from Text | FlowChartAI](https://images.openai.com/static-rsc-4/dKa2IFNwRgz7vJvf97oUFCO3Y7PMCpKABWR9vGxTkCb6OV0GwJai39tI2Qgg8Esr9xfO8rgH_KWoNTQxP7hiAx9SfZJDdX7U09cYfUBXVuy3UcWT9DQiDURopny6teHYy5NVky3uL_-WdtqAlbuL9WLVucMMvYv9fUf_VKpgdT4?purpose=inline)

En esta fase se elaboran los modelos UML y se establece la estructura de la base de datos, tomando como referencia el proyecto presentado.

Actividades principales:

- Identificar los requisitos funcionales y no funcionales.
- Elaborar los diagramas UML.
- Diseñar la base de datos.
- Definir la arquitectura de la aplicación web.
- Analizar los riesgos técnicos del proyecto.

Ejemplo de caso de uso: Confirmar pedido

El cliente selecciona los productos, revisa su carrito, elige delivery o recojo en local y registra el pago. El sistema valida la disponibilidad y confirma el pedido si se cumplen las condiciones.

### Diagrama de actividades

Inicio

Seleccionar productos

Revisar carrito

Elegir modalidad de entrega

Validar disponibilidad y pago

Confirmar pedido y generar comprobante

Fin

Resultado de la fase: se obtiene el diseño del sistema, los diagramas, el modelo de datos y una arquitectura definida que permita comenzar la programación.

## 3. Fase de Construcción

Objetivo: desarrollar las funcionalidades del sistema mediante iteraciones.

En esta fase, el diseño se convierte en un software funcional. Se construye y prueba cada módulo progresivamente.

[KI Workshop: Schnell eigene KI Use Cases entwickeln!](https://images.openai.com/static-rsc-4/NRBOuMNgs27p08cOd1BDRgLIsbcyHoQmMQsolUFDgFCsqz0PzMPdYK7K6-8WLC2B8yqyeie2V8APvhCPHEkYL0tGGycBZmHEWLCKsJhdk5yBrpJvmjhvKw_nn4Vyqs5FLZKZEUfuDbjb8R8wudbJzNVd70RxHfGYifzV468LfD8?purpose=inline)

Iteraciones propuestas para el negocio:

| Iteración         | Funcionalidades desarrolladas                                         |
| ----------------- | --------------------------------------------------------------------- |
| 1. Usuarios       | Registro, inicio de sesión y control de acceso.                       |
| 2. Carta digital  | Categorías, productos, precios y disponibilidad.                      |
| 3. Pedidos        | Carrito, personalización y confirmación del pedido.                   |
| 4. Entrega y pago | Modalidades delivery y recojo, registro del pago y comprobante.       |
| 5. Administración | Seguimiento de pedidos, gestión de productos e indicadores de ventas. |

Ejemplo práctico: durante la tercera iteración se programa el carrito. El cliente agrega dos platos y una bebida; el sistema calcula el subtotal y permite continuar a la confirmación del pedido.

Después de implementar cada módulo, se realizan pruebas para verificar que funcione correctamente y que no afecte las funcionalidades desarrolladas anteriormente.

Resultado de la fase: se obtiene una versión funcional del sistema con sus módulos integrados y probados.

## 4. Fase de Transición

Objetivo: entregar el sistema a sus usuarios y comprobar que cumpla las necesidades del restaurante.

Se verifica el funcionamiento en un entorno real o de prueba y se corrigen los problemas encontrados.

[MenuSuite - Restaurant QR ordering with staff control](https://images.openai.com/static-rsc-4/ioeaI6BDHsolpV2-4i2WIMSk3vgrTapoySVN_9KDbiMfGKwwoyeFEAxX4pBpV25_81jtesf9lflMA71TX9rW3PX0y2eJFTC1zlHsAMEnKRDnm7n-Klrk9tPourRDQWYwARi5CojjINrx0Lww_XN7RGZtZalRJFDZ2I_m9Gok4ZU?purpose=inline)

Actividades principales:

- Realizar pruebas de aceptación con clientes y personal.
- Corregir errores detectados.
- Capacitar al personal para gestionar los pedidos.
- Preparar la instalación y publicación de la aplicación web.
- Elaborar manuales de usuario y documentación técnica.

Ejemplo práctico: el restaurante realiza un pedido de prueba en modalidad delivery. El sistema debe registrar los productos, validar el pago, emitir el comprobante y permitir que el cliente consulte el estado del pedido.

También se prueba un pedido con recojo en local para verificar que no se exijan datos de envío innecesarios.

Resultado de la fase: el sistema queda validado y preparado para su puesta en funcionamiento, siempre que se hayan completado las pruebas y las condiciones de despliegue.

## 5. Cómo se aplica el ciclo iterativo de RUP

RUP no consiste solamente en completar cuatro fases de manera lineal. Dentro de ellas se realizan iteraciones que permiten evaluar los resultados y mejorar el sistema.

Inicio

Definir el problema y el alcance

Elaboración

Analizar requisitos y diseñar la arquitectura

Construcción

Programar, probar y mejorar en iteraciones

Transición

Validar, capacitar y desplegar

Si las pruebas revelan problemas, se puede regresar a una iteración anterior para corregir el diseño o la implementación.

## 6. Relación entre RUP y el proyecto del restaurante

| Elemento de RUP             | Aplicación al sistema                                                                   |
| --------------------------- | --------------------------------------------------------------------------------------- |
| Dirigido por casos de uso   | Se priorizan acciones como confirmar pedidos y consultar estados.                       |
| Centrado en la arquitectura | Se define cómo se relacionan la interfaz web, la lógica del sistema y la base de datos. |
| Orientado a riesgos         | Se analizan riesgos como pagos rechazados, productos agotados y pérdida de información. |
| Iterativo e incremental     | Se desarrolla y valida cada módulo progresivamente.                                     |

## 7. Conclusión

La metodología RUP permite organizar el desarrollo del Sistema de Pedidos con Delivery y Recojo en Local en cuatro fases. Primero se identifica la necesidad del negocio; después se analiza y diseña la solución; luego se programan y prueban los módulos; finalmente, se valida el sistema y se prepara su puesta en funcionamiento.

De esta manera, el restaurante puede reducir los errores en la toma de pedidos, mejorar el seguimiento de las entregas y administrar sus productos y ventas de forma más ordenada.

Importante: el documento del proyecto describe un prototipo en Java Swing y una propuesta web, pero señala que todavía no existe una implementación productiva completa ni una integración real con la base de datos y los servicios de pago. Por eso, las fases de construcción y transición descritas aquí son una propuesta de aplicación de RUP, no una afirmación de que todo el sistema ya esté desarrollado.

¿Quieres que también te ayude a convertir esta aplicación de RUP en un informe académico listo para presentar, con portada, objetivos, fases y diagramas UML? Puedo ayudarte a organizarlo por secciones y hacer seguimiento si necesitas terminarlo para una fecha concreta.