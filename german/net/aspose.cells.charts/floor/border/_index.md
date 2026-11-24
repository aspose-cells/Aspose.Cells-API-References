---
title: "Floor.Border"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Floor-Eigenschaft. Liest oder setzt die border Line"
type: docs
url: /de/net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Liest oder setzt die border [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FloorPropertyBorderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte den Floor des Diagramms
            Floor floor = chart.Floor;

            // Grenzeigenschaften festlegen, indem die vorhandene Grenze geändert wird, anstatt eine neue zu erstellen
            floor.Border.Color = Color.Red;
            floor.Border.Weight = WeightType.MediumLine;
            floor.Border.DashType = MsoLineDashStyle.DashDot;
            floor.Border.IsVisible = true;
            floor.Border.Transparency = 0.5;

            // Speichere die Arbeitsmappe
            workbook.Save("FloorBorderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


