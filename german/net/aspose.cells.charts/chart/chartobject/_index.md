---
title: "Chart.ChartObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Eigenschaft. Stellt das chartShape dar"
type: docs
url: /de/net/aspose.cells.charts/chart/chartobject/
---
## Chart.ChartObject property

Stellt das chartShape dar;

```csharp
public ChartShape ChartObject { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartObjectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ChartObject‑Eigenschaften demonstrieren
            chart.ChartObject.Placement = PlacementType.Move;
            chart.ChartObject.X = 100;
            chart.ChartObject.Y = 200;
            chart.ChartObject.Width = 400;
            chart.ChartObject.Height = 300;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartObjectDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [ChartShape](../../../aspose.cells.drawing/chartshape/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


