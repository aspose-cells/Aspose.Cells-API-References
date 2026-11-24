---
title: "ChartFrame.BackgroundMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Gibt den Anzeigemodus des Hintergrunds zurück und legt ihn fest. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig."
type: docs
url: /de/net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

Gibt den Anzeigemodus des Hintergrunds zurück und legt ihn fest. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode BackgroundMode { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Eigenschaft ChartFrame.Area.FillFormat.FillType. Zum Beispiel, wenn Sie den BackgroundMode auf Opaque setzen müssen, können Sie den folgenden Code verwenden: `Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red;` Diese Eigenschaft wird 12 Monate später, seit Februar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["B4"].PutValue(20);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdaten festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrieren Sie die BackgroundMode-Eigenschaft
            chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
            chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartBackgroundModeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


