---
title: ConnectionParameter clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 10
url: /es/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter clase
Especifica propiedades sobre cualquier parámetro utilizado con conexiones de datos externas
Los parámetros son válidos para ODBC y consultas web.



El tipo ConnectionParameter expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [sql_type](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | Tipo de dato SQL del parámetro Solo válido para fuentes ODBC.|
| [refresh_on_change](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Indicador que indica si la consulta debe actualizarse automáticamente cuando el contenido de un<br/> celda que proporciona los cambios de valor del parámetro. Si es verdadero, los datos externos se actualizan<br/> usando el nuevo valor del parámetro cada vez que hay un cambio.<br/> solo se actualiza cuando lo solicita el usuario, o algún otro evento activa la actualización (p. ej., libro de trabajo abierto).|
| [prompt](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Cadena de solicitud para el parámetro. Se presenta al usuario de la hoja de cálculo junto con la interfaz de usuario de entrada.<br/> para recopilar el valor del parámetro antes de actualizar los datos externos.<br/>tipo de parámetro = solicitud.|
| [type](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/type) | Tipo de parámetro utilizado.<br/> Si el tipo de parámetro = valor, entonces el valor de booleano, doble, entero,<br/> o se usará una cadena.<br/> Se especificará {booleano, doble, entero o cadena}.|
| [name](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/name) | El nombre del parámetro.|
| [cell_reference](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell referencia que indica qué valor de celda usar para el parámetro de consulta. Se usa solo cuando el tipo de parámetro es celda.|
| [value](/cells/es/python-net/aspose.cells.externalconnections/connectionparameter/value) | Valor numérico no entero, valor entero, valor de cadena o valor booleano<br/> para usar como parámetro de consulta.|



###  Ver también
* módulo [aspose.cells.externalconnections](..)
