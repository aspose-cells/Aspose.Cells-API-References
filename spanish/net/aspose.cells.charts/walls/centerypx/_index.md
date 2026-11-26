---
title: "Walls.CenterYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Walls. Obtiene la coordenada y de la esquina inferior izquierda del centro de Wall en unidades de píxeles después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/walls/centerypx/
---
## Walls.CenterYPx property

Obtiene la coordenada y de la esquina inferior izquierda del centro de la pared en unidades de píxeles después de llamar al método Chart.Calculate().

```csharp
public int CenterYPx { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYPxDemo
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

            chart.Calculate();

            Walls walls = chart.Walls;
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);

            workbook.Save("WallsPropertyCenterYPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


