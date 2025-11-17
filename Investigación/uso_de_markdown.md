## **Qué es Markdown**

Markdown es un lenguaje de marcado ligero creado por John Gruber y Aaron Swartz en 2004. Su principal objetivo es que el texto plano sea lo más legible posible, tanto en su forma de entrada (el código) como una vez renderizado (la salida). Permite a los usuarios escribir contenido utilizando una sintaxis sencilla y fácil de entender —como asteriscos para negritas o guiones para listas— que luego se puede convertir en HTML u otros formatos para su visualización. Esto significa que puedes dar formato (encabezados, listas, enlaces, etc.) a tu texto usando caracteres simples sin la complejidad del HTML o un procesador de texto pesado.



## **Uso en Proyectos de Software** 

En proyectos de software, Markdown se utiliza extensamente por varias razones clave, principalmente para la documentación:



##### Archivos README

&nbsp;Casi todos los proyectos de software incluyen un archivo README.md (la extensión .md o .markdown indica el formato Markdown) que es lo primero que ve un usuario o colaborador. Este archivo describe el proyecto, cómo instalarlo y cómo usarlo.



##### Documentación General

&nbsp;Es el formato preferido para archivos de contribución (CONTRIBUTING.md), licencias (LICENSE.md), guías básicas y documentación interna.



##### Sistemas de Control de Versiones

&nbsp;Plataformas como GitHub, GitLab y Bitbucket renderizan archivos Markdown directamente, haciéndolos legibles y con buen formato sin necesidad de pasos adicionales.



#### Markdown y GitHub

&nbsp;Sinergia, Ventajas y Desventajas 

GitHub utiliza una versión extendida de Markdown llamada GitHub Flavored Markdown (GFM). Esto permite características adicionales como listas de tareas (checkboxes), tablas, resaltado de sintaxis de código y menciones de usuarios, lo que lo hace ideal para la colaboración y la documentación técnica.



## **Ventajas de usar Markdown con GitHub** 

##### Legibilidad Universal

Los archivos son legibles incluso en texto plano, pero GitHub los convierte automáticamente en páginas web atractivas y bien estructuradas (por ejemplo, el README en la página principal del repositorio).



##### Simplicidad y Velocidad

&nbsp;Es mucho más rápido escribir documentación en Markdown que en HTML o con un editor WYSIWYG, lo que acelera el proceso de documentación.



##### Control de Versiones Efectivo

&nbsp;Como los archivos Markdown son solo texto plano, los sistemas como Git pueden rastrear y gestionar los cambios (diferencias o diffs) de manera muy eficiente.



Soporte de Características Avanzadas: GFM soporta la sintaxis de GitHub para referencias a issues y pull requests (#123), lo cual es crucial para la gestión de proyectos.



## **Desventajas de usar Markdown con GitHub** 

##### Funcionalidad Limitada

Markdown, por diseño, es simple. Si necesitas un diseño muy complejo, scripts incrustados o interactividad avanzada, Markdown no es suficiente y tendrás que recurrir a HTML o un generador de sitios estáticos más potente.



##### Estandarización Variable

&nbsp;Aunque GFM es muy popular, hay variaciones entre diferentes implementaciones de Markdown. Lo que funciona en GitHub podría no renderizarse exactamente igual en otra plataforma.



##### Dependencia de la Plataforma

&nbsp;Para la mejor experiencia visual, dependes de que GitHub renderice el archivo. Si el archivo se visualiza en un entorno que no es GitHub, se verá solo como texto plano con los caracteres de formato visibles.

