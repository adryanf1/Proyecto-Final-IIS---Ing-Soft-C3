# Resumen del Sistema de Control de Asistencia

## Descripción del Caso y Alcance

El sistema de control de asistencia es una aplicación cuyo propósito principal es permitir a los profesores registrar y revisar la asistencia de los estudiantes a sus clases de una forma sencilla y rápida, dejando de lado el uso de listas de papel.

El alcance de la aplicación es específico para el control de asistencia (Caso 5). Este incluye:

* Registrar asistencias (RF1).
* Ver el historial individual (RF3).
* Cambiar un registro si se cometió un error (RF4).
* Generar reportes simples de porcentaje de asistencia (RF5).

El sistema está diseñado para ser fácil de usar y funcionar bien en dispositivos móviles como celulares o tabletas (RNF3).

**Funcionalidades excluidas:** la aplicación no incluye gestión de notas, control de inventario ni programación avanzada de horarios.



## Objetivos del Sistema

El objetivo de definir los requerimientos es establecer:

* Lo que el sistema **debe hacer** (Requerimientos Funcionales).
* Las **características de calidad** que debe cumplir (Requerimientos No Funcionales).

El propósito general es permitir a los profesores registrar y revisar la asistencia de forma rápida y sencilla.



## Requerimientos Clave

### Requerimientos Funcionales (RF)

* **RF1 – Registro de Asistencia:** Permite marcar asistencia como *presente*, *ausente* o *justificado*.
* **RF3 – Historial Individual:** Permite ver el historial de un estudiante.
* **RF4 – Modificación de Registro:** Permite corregir una entrada, como cambiar “ausente” a “justificado”.
* **RF5 – Reportes:** Genera un reporte con el porcentaje total de asistencia.



### Requerimientos No Funcionales (RNF)

* **RNF1 – Seguridad:** Solo profesores autorizados pueden acceder mediante inicio de sesión.
* **RNF2 – Rendimiento:** Registrar una clase (≈30 estudiantes) debe tomar menos de 5 segundos.
* **RNF3 – Usabilidad móvil:** La interfaz debe ser usable en teléfonos y tabletas.



## Casos de Prueba (sin tabla)

A continuación se describen los casos de prueba sin formato de tabla:

* **CP01**

  * Tipo: Unitario
  * Requerimiento: RF1
  * Datos: Profesor selecciona curso → estudiante “Ana Soto” → marca “Presente”.
  * Resultado esperado: Confirmación y estado actualizado.
  * Resultado obtenido: Éxito.

* **CP03**

  * Tipo: Unitario
  * Requerimiento: RNF1
  * Datos: Contraseña ingresada: “Incorrecta123”.
  * Resultado esperado: Mensaje “Credenciales incorrectas” y acceso denegado.
  * Resultado obtenido: Éxito.

* **CP04**

  * Tipo: Validación
  * Requerimiento: RNF2
  * Datos: Registro de asistencia para 35 estudiantes.
  * Resultado esperado: Tiempo de guardado ≤ 5 segundos.
  * Resultado obtenido: Éxito.

* **CP05**

  * Tipo: Validación
  * Requerimiento: RF5
  * Datos: Reporte final. Estudiante “María Gómez”: 10 asistencias de 20 clases.
  * Resultado esperado: Porcentaje mostrado: **50%**.
  * Resultado obtenido: Éxito.



## Tipo de Mantenimiento Propuesto

Los problemas señalados y su mantenimiento correspondiente se describen así:

* **Problema:** Seguridad vaga y riesgosa (acceso insuficiente).

  * Tipo: **Preventivo**
  * Acción: Uso de contraseñas robustas y mejor gestión de sesiones.
  * Justificación: Evita problemas futuros y mejora la seguridad general.

* **Problema:** Seguridad vaga y riesgosa (debilidad adicional de acceso).

  * Tipo: **Perfectivo**
  * Acción: Añadir autenticación multifactor (2FA).
  * Justificación: Incrementa la seguridad y mejora la mantenibilidad.

* **Problema:** Reportes tardíos y poco útiles (solo al final del semestre).

  * Tipo: **Perfectivo**
  * Acción: Crear un módulo de alertas de ausencias frecuentes.
  * Justificación: Permite intervención temprana y mejora la utilidad del sistema.



## Reflexión sobre el Control de Versiones

El control de versiones es fundamental para el desarrollo del Sistema de Control de Asistencia porque permite llevar un registro claro de todos los cambios realizados, desde la definición de requerimientos hasta la ejecución de pruebas. Gracias a los commits, es posible identificar qué se modificó y corregir errores sin perder información importante.



Subir el proyecto a GitHub fortalece este proceso, ya que ofrece un historial organizado, comparación entre versiones y un lugar seguro donde almacenar el avance del sistema. Además, permite mantener la coherencia entre los requerimientos establecidos y las mejoras realizadas a lo largo del tiempo. En conjunto, el control de versiones y GitHub aseguran que el sistema evolucione de manera ordenada, confiable y fácil de mantener.

