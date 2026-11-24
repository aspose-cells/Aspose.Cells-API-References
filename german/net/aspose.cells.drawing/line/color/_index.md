---
title: "Line.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line‑Eigenschaft. Stellt die Farbe der Linie dar"
type: docs
url: /de/net/aspose.cells.drawing/line/color/
---
## Line.Color property

Stellt die Farbe der Linie dar.

```csharp
public Color Color { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyColorDemo
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
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Achsenlinienfarben festlegen
            chart.CategoryAxis.AxisLine.Color = Color.BlueViolet;
            chart.ValueAxis.AxisLine.Color = Color.BlueViolet;
            
            // Schriftfarbe des Achsentitels festlegen
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.Font.Color = Color.BlueViolet;

            // Speichere die Arbeitsmappe
            workbook.Save("LinePropertyColorDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


