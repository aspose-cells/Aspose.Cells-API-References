---
title: "ChartFrame.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame‑Eigenschaft. Gibt ein Font‑Objekt des angegebenen ChartFrame‑Objekts zurück"
type: docs
url: /de/net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Gibt ein `Font`-Objekt des angegebenen ChartFrame-Objekts zurück.

```csharp
public virtual Font Font { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyFontDemo
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

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze Diagrammtitel und konfiguriere die Schriftarteigenschaften
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            chart.Title.Font.Color = System.Drawing.Color.Blue;
            chart.Title.Font.CapsType = TextCapsType.None;
            chart.Title.Font.IsBold = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


