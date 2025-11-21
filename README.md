# Resumen del sistema Agenda personal de citas
## Descripcion del caso

El sistema de Agenda personal de citas es una app cuyo proposito es tener mas organizacion y gestionar compromisos de manera eficiente, ayudando al usuario a tener un control ordenado de su tiempo y evitar conflictos entre horarios




## Objetivos del sistema

 Los objetivos del sistema: 
  
  * Lo que el sistema **"Debe hacer"** (RF)
  * Las **"caracteristicas"** que debe cumplir (RNF)



## Requerimientos

### Requerimientos funcionales  (RF)
* **RF1 - Crear cita con recordatorio automatico:** El sistema debe permitir al usuario configurar un recordatorio que se active antes de la cita.
* **RF2 - Clasificacion de citas por categoria:** El usuario puede asignar categorías como **“Salud”**, **“Trabajo”**, **“Personal”** a cada cita.
* **RF3 - Visualizacion semanal y mensual:** El sistema debe mostrar las citas en vistas de calendario semanal y mensual.
* **RF3 - Exportacion de citas a PDF** El usuario puede exportar sus citas filtradas por rango de fecha en formato PDF.



### Requerimientos no funcionales (RNF)
* **RNF1 - Compatibilidad multiplataforma:** La aplicación debe funcionar correctamente en dispositivos móviles y de escritorio.
* **RNF2 - Seguridad de datos:** Las citas deben almacenarse de forma segura, con cifrado básico en el almacenamiento local.
* **RNF3 - Rendimiento:** El sistema debe cargar la vista mensual en menos de 2 segundos con hasta 100 citas registradas. 


## Casos de prueba (Sin tabla)

* **CP1**

  * Tipo: Unitario
  * Requerimiento: RF1
  * Datos: **Fecha:** Usuario Ingresa fecha **Hora:** Usuario ingresa hora
  * Resutado esperado: Cita registrada con recordatorio
  * Resultado obtenido: Cita con notificacion 30 minutos antes (Exito)


* **CP3**

  * Tipo: Unitario
  * Requerimiento: RF2
  * Datos: **Categoria:** Usuario Ingresa Categoria "Consulta"
  * Resutado esperado: Cita aparece con el color asignado a la categoria
  * Resultado obtenido: Cita con etiqueta de color rojo (Exito)


* **CP4**

  * Tipo: Validacion
  * Requerimiento: RNF2
  * Datos: **Usuario:** Usuario Ingresa Usuario **Contraseña:** Usuario ingresa Contraseña
  * Resutado esperado: Acceso conseguido
  * Resultado obtenido: Otorgado (Exito)


* **CP5**

  * Tipo: Validacion
  * Requerimiento: RF5
  * Datos: **Rango de citas:** Usuario ingresa el rango de citas
  * Resutado esperado: Archivo PDF generado con las citas
  * Resultado obtenido: Archivo generado con 3 citas (Exito)



## Tipos de propuesta de mantenimiento 

* **Problema:** El sistema esta poco actualizado teniendo problemas de carga al tener el historial de citas mal optimizado.
 
 
  * **Tipo de Mantenimiento:** Mantenimiento correctivo
  * **Accion:** Optimizar la consulta y carga del historial mediante filtros avanzados y mejoras en la consulta a la base de datos.
  * **Justificacion:** Es una mejora necesaria para evitar futuros problemas o caidas de servidores por mala optimizacion.


* **Problema:** El sistema no permite realizar cambios de personalizacion como los ajustes de apariencia (como el modo oscuro o claro) lo que limita la comodidad y accesibilidad del usuario.
 

 
  * **Tipo de Mantenimiento:** Mantenimiento Perfectivo
  * **Accion:** Agregar una opcion de personalizacion que permita interfaz de modo oscuro/claro, seleccion de paleta de colores y ajustes basicos de apariencia.
  * **Justificacion:** Es requerida para la mejora de los estandares de usabilidad y accesibilidad, lo que permite que el sistema se adapte a preferencias visuales del usuario.


## Reflexion sobre el control de versiones 

El control de versiones en el sistema de Agenda personal de citas es fundamental ya que este permite llevar el registro de los cambios realizados en cada version, desde sus inicios como lo es la definicion de requisitos hasta la ejecucion de las pruebas, asi mismo como gracias a los commits que es posible indentificar que errores se corrigio sin perder la informacion importante.

El subir este proyecto a Github ofrece muchas ventajas, ya que es un lugar seguro donde almacenar el avance del sistema, asi mismo, permite mantener la coherencia entre las mejoras realizadas a lo largo del tiempo.
