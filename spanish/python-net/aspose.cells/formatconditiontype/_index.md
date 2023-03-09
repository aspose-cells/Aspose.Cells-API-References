---
title: FormatConditionType enumeración
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 2100
url: /es/python-net/aspose.cells/formatconditiontype/
is_root: false
---
##  FormatConditionType enumeración
Tipo de regla de formato condicional.



El tipo FormatConditionType expone los siguientes miembros:

###  Campos
| Campo| Descripción|
| :- | :- |
| CELL_VALUE | Esta regla de formato condicional compara un valor de celda<br/> a un resultado calculado con una fórmula, usando un operador.|
| EXPRESSION | Esta regla de formato condicional contiene una fórmula para<br/>evaluar.Cuando el resultado de la fórmula es verdadero, la celda es<br/> resaltado.|
| COLOR_SCALE | Esta regla de formato condicional crea un<br/> escala de colores en las celdas.|
| DATA_BAR | Esta regla de formato condicional muestra una calificación<br/> barra de datos en el rango de celdas.|
| ICON_SET |Esta regla de formato condicional aplica iconos a las celdas<br/> según sus valores.|
| TOP10 | Esta regla de formato condicional resalta las celdas cuyas<br/>los valores caen en el soporte N superior o N inferior, como<br/> especificado.|
| UNIQUE_VALUES | Esta regla de formato condicional destaca<br/> valores en el rango.|
| DUPLICATE_VALUES | Esta regla de formato condicional resalta los duplicados<br/> valores.|
| CONTAINS_TEXT | Esta regla de formato condicional resalta las celdas<br/>que contiene el texto dado. Equivalente a usar SEARCH()<br/>función de hoja para determinar si la celda contiene<br/> el texto.|
| NOT_CONTAINS_TEXT | Esta regla de formato condicional resalta las celdas que<br/>no contienen texto dado.<br/>función de hoja para determinar si la celda contiene<br/> el texto o no.|
| BEGINS_WITH | Esta regla de formato condicional resalta las celdas en el<br/>rango que comienza con el texto dado.<br/> usando la función de hoja LEFT() y comparando valores.|
| ENDS_WITH | Esta regla de formato condicional resalta las celdas que terminan<br/>con el texto dado Equivalente a usar la hoja DERECHA()<br/> función y comparación de valores.|
| CONTAINS_BLANKS | Esta regla de formato condicional resalta las celdas que<br/>están completamente en blanco Equivalente a usar LEN(TRIM()).<br/>Esto significa que si la celda contiene solo caracteres<br/>que TRIM() eliminaría, entonces se considera en blanco.<br/> Una celda vacía también se considera en blanco.|
| NOT_CONTAINS_BLANKS | Esta regla de formato condicional resalta las celdas que<br/>no están en blanco Equivalente a usar LEN(TRIM()).<br/>significa que si la celda contiene sólo caracteres que<br/>TRIM() eliminaría, entonces se considera en blanco.<br/> las celdas vacías también se consideran en blanco.|
| CONTAINS_ERRORS | Esta regla de formato condicional resalta las celdas con<br/>errores de fórmula Equivalente a usar la hoja ISERROR()<br/> función para determinar si hay un error de fórmula.|
| NOT_CONTAINS_ERRORS | Esta regla de formato condicional resalta las celdas<br/>sin errores de fórmula Equivalente a usar ISERROR()<br/> función de hoja para determinar si hay un error de fórmula.|
| TIME_PERIOD | Esta regla de formato condicional resalta las celdas<br/>que contienen fechas en el período de tiempo especificado.<br/>valor subyacente de la celda se evalúa, por lo tanto, el<br/>la celda no necesita ser formateada como una fecha para ser<br/>Por ejemplo, con una celda que contiene el<br/>valor 38913 se aplicará el formato condicional si<br/> la regla requiere un valor de 14/7/2006.|
| ABOVE_AVERAGE | Esta regla de formato condicional resalta las celdas que<br/>están por encima o por debajo del promedio para todos los valores en el<br/> rango.|



###  Ver también
* módulo [aspose.cells](..)
