---
title: AccessCacheOptions enumeración
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1740
url: /es/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
##  AccessCacheOptions enumeración
Opciones de caché para acceso a datos. Se puede combinar con el operador | para múltiples opciones juntas.



El tipo AccessCacheOptions expone los siguientes miembros:

###  Campos
| Campo| Descripción|
| :- | :- |
| NONE | Sin caché para ningún acceso a datos.|
| ALL | Aplique todas las optimizaciones posibles para todo tipo de acceso a datos en el libro de trabajo.<br/> Todas las configuraciones y datos no deben cambiarse durante el acceso optimizado.|
| POSITION_AND_SIZE | Aplique la posible optimización para obtener la posición y el tamaño del objeto (como la forma).<br/>La configuración de altura de fila y ancho de columna no debe cambiarse durante el acceso optimizado.|
| CELLS_DATA | Aplique la posible optimización para obtener los valores de las celdas.<br/>Los datos Cells (datos y configuraciones de Cell, Fila) no deben cambiarse durante<br/>el acceso optimizado, tampoco se deben crear nuevos objetos Cell/Row (como<br/> por [[indexador]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CELL_DISPLAY | Aplique la posible optimización para obtener resultados relacionados con la visualización de<br/>celdas ([Cell.display_string_value](/cells/es/python-net/aspose.cells/cell#display_string_value), [Cell.get_style()](/cells/es/python-net/aspose.cells/cell/get_style), [Cell.get_display_style()](/cells/es/python-net/aspose.cells/cell/get_display_style), etc.).<br/>Cells Los datos y los objetos relacionados con el estilo (Cell/Estilos de fila/columna, ancho de columna, etc.) no deben cambiarse<br/> durante el acceso optimizado.|
| GET_FORMULA | Aplicar la posible optimización para obtener fórmulas.<br/>Todos los datos y configuraciones que pueden afectar la expresión de la fórmula (nombre de la hoja de trabajo, texto del nombre,<br/> columnas de la tabla, etc.) no deben cambiarse durante el acceso optimizado.|
| SET_FORMULA | Aplicar posibles optimizaciones para establecer fórmulas.<br/>Todos los datos y configuraciones que pueden afectar la expresión de la fórmula (nombre de la hoja de trabajo, texto del nombre,<br/> columnas de la tabla, etc.) no deben cambiarse durante el acceso optimizado.|
| CALCULATE_FORMULA |Aplicar posibles optimizaciones para el cálculo de fórmulas.<br/>Los datos Cells no deben cambiarse durante el acceso optimizado, ningún objeto nuevo (Cell, Fila, etc.)<br/> debe crearse (como por [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CONDITIONAL_FORMATTING | Aplique la posible optimización para obtener resultados de formato de formatos condicionales.<br/>Todos los datos y configuraciones que puedan afectar el resultado de los formatos condicionales (configuraciones de<br/> formatos condicionales, valores de celda dependientes, etc.) no deben cambiarse durante el acceso optimizado.|
| VALIDATION | Aplique la posible optimización para obtener resultados de validación.<br/>Todos los datos y configuraciones que puedan afectar el resultado de la validación (configuraciones de la validación,<br/> valores de celda dependientes, etc.) no deben cambiarse durante el acceso optimizado.|



###  Observaciones

Para algunas funciones, acceder a grandes conjuntos de datos requiere muchas operaciones repetitivas y complicadas
como búsqueda, cálculo, etc., y esas operaciones llevarán mucho tiempo extra.
Para situaciones comunes, todos los datos dependientes permanecen sin cambios durante el acceso, por lo que algunos cachés se pueden construir y usar para
mejorar el rendimiento de acceso.
Para este propósito, proporcionamos este API para que el usuario pueda especificar qué tipo de acceso a los datos necesita.
para ser optimizado por un posible mecanismo de almacenamiento en caché.


Tenga en cuenta que, para diferentes opciones, es posible que se requiera que diferentes conjuntos de datos sean de "solo lectura".
Y el rendimiento del acceso a los datos depende de muchos aspectos, el uso del mecanismo de almacenamiento en caché
no garantiza que se mejorará el rendimiento.
como el conjunto de datos al que se accede es pequeño, el uso de la memoria caché puede llevar aún más tiempo porque
el almacenamiento en caché también necesita cierto tiempo adicional.

###  Ver también
* módulo [aspose.cells](..)
