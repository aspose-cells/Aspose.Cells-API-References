---
title: "Area.BackgroundColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Area‑Eigenschaft. Gibt die Hintergrundfarbe des Area zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Gibt die Hintergrundfarbe des [`Area`](../) zurück oder legt sie fest.

```csharp
public Color BackgroundColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
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

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Hintergrundfarbe für den Kategorienachsenbereich festlegen
            chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;

            // Zeigt die Hintergrundfarbe an
            Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);

            // Speichere die Arbeitsmappe
            workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


