---
title: "Clase AboveAverage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AboveAverage. Describe la regla de formato condicional AboveAverage. Esta regla de formato condicional resalta celdas que están por encima o por debajo del promedio para todos los valores en el rango."
type: docs
url: /es/net/aspose.cells/aboveaverage/
---
## AboveAverage class

Describe la regla de formato condicional AboveAverage. Esta regla de formato condicional resalta las celdas que están por encima o por debajo del promedio de todos los valores en el rango.

```csharp
public class AboveAverage
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AboveAverage](aboveaverage/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Obtenga o establezca la bandera que indica si la regla es una regla "above average". 'true' indica "above average". El valor predeterminado es true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Obtenga o establezca la bandera que indica si los criterios 'aboveAverage' y 'belowAverage' son inclusivos del promedio mismo, o exclusivos de ese valor. 'true' indica incluir el valor promedio en los criterios. El valor predeterminado es false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Obtenga o establezca el número de desviaciones estándar para incluir por encima o por debajo del promedio en la regla de formato condicional. El valor de entrada debe estar entre 0 y 3 (incluyendo 0 y 3). Establecer este valor en 0 significa que stdDev no está configurado. El valor predeterminado es 0. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Agregar una colección de formato condicional a la hoja de cálculo
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Definir el área de celdas donde aplicar el formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Agregar una condición por encima del promedio a la colección
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Establecer el color de fondo para la condición
            fc.Style.BackgroundColor = Color.Yellow;

            // Establecer propiedades para la condición por encima del promedio
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Guarda el libro de trabajo
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


