---
title: RenameStrategy enumeración
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 2430
url: /es/python-net/aspose.cells/renamestrategy/
is_root: false
---
##  RenameStrategy enumeración
Opción de estrategia para nombres duplicados de columnas.



El tipo RenameStrategy expone los siguientes miembros:

###  Campos
| Campo| Descripción|
| :- | :- |
| EXCEPTION | Lanza una excepción.|
| DIGIT | Nombrado con dígito. Los nombres duplicados se convertirán en ...1, ...2, etc.|
| LETTER | Nombrado con letra.. Los nombres duplicados se convertirán en ...A, ...B, etc.|



###  Observaciones

Al procesar datos con encabezados, algunos escenarios requieren que los encabezados no se dupliquen para todas las columnas.
Por ejemplo, al exportar datos a una tabla de datos y se requiere que el encabezado se tome como el nombre de la columna de la tabla de datos,
los valores duplicados del encabezado no son válidos.
Para este tipo de situaciones, el usuario puede determinar cómo manejarlas especificando esta estrategia.

###  Ver también
* módulo [aspose.cells](..)
