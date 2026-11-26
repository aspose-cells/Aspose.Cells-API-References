---
title: "Enumeración FormatConditionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridDesktop.FormatConditionType enum. Tipo de regla de formato condicional"
type: docs
url: /es/net/aspose.cells.griddesktop/formatconditiontype/
---
## FormatConditionType enumeration

Tipo de regla de formato condicional.

```csharp
public enum FormatConditionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| CellValue | `0` | Esta regla de formato condicional compara el valor de una celda con el resultado calculado de una fórmula, utilizando un operador. |
| Expression | `1` | Esta regla de formato condicional contiene una fórmula para evaluar. Cuando el resultado de la fórmula es verdadero, la celda se resalta. |
| ColorScale | `2` | Esta regla de formato condicional crea una escala de colores graduada en las celdas. |
| DataBar | `3` | Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas. |
| IconSet | `4` | Esta regla de formato condicional aplica íconos a las celdas según sus valores. |
| Top10 | `5` | Esta regla de formato condicional resalta celdas cuyos valores se encuentran en el rango superior N o inferior N, según se especifique. |
| UniqueValues | `6` | Esta regla de formato condicional resalta valores únicos en el rango. |
| DuplicateValues | `7` | Esta regla de formato condicional resalta valores duplicados. |
| ContainsText | `8` | Esta regla de formato condicional resalta celdas que contienen el texto especificado. Equivalente a usar la función de hoja SEARCH() para determinar si la celda contiene el texto. |
| NotContainsText | `9` | Esta regla de formato condicional resalta celdas que no están en blanco. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, se considera en blanco. Una celda vacía también se considera en blanco. |
| BeginsWith | `10` | Esta regla de formato condicional resalta celdas en el rango que comienzan con el texto especificado. Equivalente a usar la función de hoja LEFT() y comparar valores. |
| EndsWith | `11` | Esta regla de formato condicional resalta celdas que terminan con el texto especificado. Equivalente a usar la función de hoja RIGHT() y comparar valores. |
| ContainsBlanks | `12` | Esta regla de formato condicional resalta celdas que están completamente en blanco. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, se considera en blanco. Una celda vacía también se considera en blanco. |
| NotContainsBlanks | `13` | Esta regla de formato condicional resalta celdas que no están en blanco. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, se considera en blanco. Una celda vacía también se considera en blanco. |
| ContainsErrors | `14` | Esta regla de formato condicional resalta celdas con errores de fórmula. Equivalente a usar la función de hoja ISERROR() para determinar si hay un error de fórmula. |
| NotContainsErrors | `15` | Esta regla de formato condicional resalta celdas sin errores de fórmula. Equivalente a usar la función de hoja ISERROR() para determinar si hay un error de fórmula. |
| TimePeriod | `16` | Esta regla de formato condicional resalta celdas que contienen fechas en el período de tiempo especificado. El valor subyacente de la celda se evalúa, por lo tanto la celda no necesita estar formateada como fecha para ser evaluada. Por ejemplo, con una celda que contiene el valor 38913, el formato condicional se aplicará si la regla requiere un valor de 7/14/2006. |
| AboveAverage | `17` | Esta regla de formato condicional resalta celdas que están por encima o por debajo del promedio de todos los valores en el rango. |

### Ver también

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


