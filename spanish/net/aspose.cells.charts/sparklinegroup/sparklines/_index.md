---
title: "SparklineGroup.Sparklines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene la colección de objetos Sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/sparklines/
---
## SparklineGroup.Sparklines property

Obtiene la colección del objeto [`Sparkline`](../../sparkline/).

```csharp
public SparklineCollection Sparklines { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySparklinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Crear grupo de sparkline
            CellArea location = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 4, EndColumn = 4 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Agregar sparkline usando la propiedad Sparklines
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personalizar la apariencia del sparkline
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Guarda el libro de trabajo
            workbook.Save("SparklineDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


