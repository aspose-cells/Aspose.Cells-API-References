---
title: "Chart.Placement"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart propiedad. Representa la forma en que el gráfico está unido a las celdas debajo de él"
type: docs
url: /es/net/aspose.cells.charts/chart/placement/
---
## Chart.Placement property

Representa la forma en que el gráfico está unido a las celdas debajo de él.

```csharp
public PlacementType Placement { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlacementDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregue un gráfico y establezca los datos
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Demostrar la propiedad Placement
            chart.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Chart Placement: " + chart.Placement);

            workbook.Save("ChartPlacementDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


