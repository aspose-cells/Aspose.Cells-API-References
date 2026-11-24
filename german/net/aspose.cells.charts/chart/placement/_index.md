---
title: "Chart.Placement"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt an, wie das Diagramm an den darunterliegenden Zellen befestigt ist"
type: docs
url: /de/net/aspose.cells.charts/chart/placement/
---
## Chart.Placement property

Stellt dar, wie das Diagramm an den darunterliegenden Zellen befestigt ist.

```csharp
public PlacementType Placement { get; set; }
```

### Beispiele

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

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Diagramm hinzufügen und Daten festlegen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Placement-Eigenschaft demonstrieren
            chart.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Chart Placement: " + chart.Placement);

            workbook.Save("ChartPlacementDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


