---
title: "ChartPoint.Area"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt die Fläche zurück"
type: docs
url: /de/net/aspose.cells.charts/chartpoint/area/
---
## ChartPoint.Area property

Gibt die ` area` zurück.

```csharp
public Area Area { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["A5"].PutValue("D");
            
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Greifen Sie auf den ersten Punkt in der ersten Serie zu und setzen Sie Flächeneigenschaften
            Aspose.Cells.Charts.ChartPoint point = chart.NSeries[0].Points[0];
            point.Area.ForegroundColor = System.Drawing.Color.Red;
            point.Area.FillFormat.Texture = TextureType.Granite;
            point.Area.Formatting = FormattingType.Custom;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


