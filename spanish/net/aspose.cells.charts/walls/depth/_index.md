---
title: "Walls.Depth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Walls. Obtiene la profundidad de adelante a atrás en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate."
type: docs
url: /es/net/aspose.cells.charts/walls/depth/
---
## Walls.Depth property

Obtiene la profundidad de adelante hacia atrás en unidades de 1/4000 del ancho del gráfico después de llamar al método Chart.Calculate().

```csharp
public int Depth { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyDepthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            Walls walls = chart.Walls;
            Console.WriteLine("Wall Depth: " + walls.Depth);

            workbook.Save("WallsDepthExample.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


