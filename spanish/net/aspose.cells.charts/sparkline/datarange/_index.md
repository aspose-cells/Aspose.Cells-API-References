---
title: "Sparkline.DataRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Sparkline. Representa el rango de datos del sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparkline/datarange/
---
## Sparkline.DataRange property

Representa el rango de datos del sparkline.

```csharp
public string DataRange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyDataRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(7);
            sheet.Cells["A4"].PutValue(2);
            sheet.Cells["A5"].PutValue(9);

            // Agregar un grupo de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Acceda al primer sparkline y muestre su rango de datos
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline DataRange: " + sparkline.DataRange);
        }
    }
}
```

### Ver también

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


