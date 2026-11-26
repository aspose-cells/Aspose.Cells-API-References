---
title: "Enumeración FormatConditionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.FormatConditionType. Tipo de regla de formato condicional"
type: docs
url: /es/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Tipo de regla de formato condicional.

```csharp
public enum FormatConditionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| CellValue | `1` | Esta regla de formato condicional compara el valor de una celda con el resultado calculado de una fórmula, utilizando un operador. |
| Expression | `2` | Esta regla de formato condicional contiene una fórmula para evaluar. Cuando el resultado de la fórmula es verdadero, la celda se resalta. |
| Top10 | `4` | Esta regla de formato condicional resalta celdas cuyos valores se encuentran en el rango superior N o inferior N, según se especifique. |
| UniqueValues | `8` | Esta regla de formato condicional resalta valores únicos en el rango. |
| DuplicateValues | `16` | Esta regla de formato condicional resalta valores duplicados. |
| ContainsText | `32` | Esta regla de formato condicional resalta celdas que contienen el texto especificado. Equivalente a usar la función de hoja SEARCH() para determinar si la celda contiene el texto. |
| NotContainsText | `64` | Esta regla de formato condicional resalta celdas que no contienen el texto especificado. Equivalente a usar la función de hoja SEARCH() para determinar si la celda contiene el texto o no. |
| BeginsWith | `128` | Esta regla de formato condicional resalta celdas en el rango que comienzan con el texto especificado. Equivalente a usar la función de hoja LEFT() y comparar valores. |
| EndsWith | `256` | Esta regla de formato condicional resalta celdas que terminan con el texto especificado. Equivalente a usar la función de hoja RIGHT() y comparar valores. |
| ContainsBlanks | `512` | Esta regla de formato condicional resalta celdas que están completamente en blanco. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, se considera en blanco. Una celda vacía también se considera en blanco. |
| NotContainsBlanks | `1024` | Esta regla de formato condicional resalta celdas que no están en blanco. Equivalente a usar LEN(TRIM()). Esto significa que si la celda contiene solo caracteres que TRIM() eliminaría, se considera en blanco. Una celda vacía también se considera en blanco. |
| ContainsErrors | `2048` | Esta regla de formato condicional resalta celdas con errores de fórmula. Equivalente a usar la función de hoja ISERROR() para determinar si hay un error de fórmula. |
| NotContainsErrors | `4096` | Esta regla de formato condicional resalta celdas sin errores de fórmula. Equivalente a usar la función de hoja ISERROR() para determinar si hay un error de fórmula. |
| TimePeriod | `8192` | Esta regla de formato condicional resalta celdas que contienen fechas en el período de tiempo especificado. El valor subyacente de la celda se evalúa, por lo tanto la celda no necesita estar formateada como fecha para ser evaluada. Por ejemplo, con una celda que contiene el valor 38913, el formato condicional se aplicará si la regla requiere un valor de 7/14/2006. |
| AboveAverage | `16384` | Esta regla de formato condicional resalta celdas que están por encima o por debajo del promedio de todos los valores en el rango. |
| ColorScale | `32768` | Esta regla de formato condicional crea una escala de colores graduada en las celdas. |
| DataBar | `65536` | Esta regla de formato condicional muestra una barra de datos graduada en el rango de celdas. |
| IconSet | `131072` | Esta regla de formato condicional aplica íconos a las celdas según sus valores. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Crear un nuevo libro de trabajo.
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo.
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establece el rango del formato condicional.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Agrega una condición para AboveAverage
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // Estableciendo propiedades para AboveAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Agrega una condición para CellValue
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // Agrega una condición para ContainsText
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Guardar el archivo Excel
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


