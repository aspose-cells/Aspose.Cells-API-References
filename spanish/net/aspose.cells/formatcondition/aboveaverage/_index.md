---
title: "FormatCondition.AboveAverage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene la instancia AboveAverage de los formatos condicionales. La regla predeterminada de la instancia resalta las celdas que están por encima del promedio de todos los valores en el rango. Válido solo para el tipo AboveAverage"
type: docs
url: /es/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Obtenga la instancia "AboveAverage" del formato condicional. La regla de la instancia predeterminada resalta celdas que están por encima del promedio para todos los valores en el rango. Válido solo para type = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Agregar formato condicional por encima del promedio
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Establecer para resaltar valores por encima del promedio
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Agregar formato condicional por debajo del promedio
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Establecer para resaltar valores por debajo del promedio
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Guarda el libro de trabajo
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


