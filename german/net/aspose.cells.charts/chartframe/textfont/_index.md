---
title: "ChartFrame.TextFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame‑Eigenschaft. Gibt ein Font‑Objekt des angegebenen ChartFrame‑Objekts zurück"
type: docs
url: /de/net/aspose.cells.charts/chartframe/textfont/
---
## ChartFrame.TextFont property

Gibt ein [`Font`](../font/)‑Objekt des angegebenen ChartFrame‑Objekts zurück.

```csharp
[Obsolete("Use ChartFrame.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die ChartFrame.Font‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit JANUAR 2012, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyTextFontDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze Diagrammtitel und konfiguriere die Schriftart
            chart.Title.Text = "Sample Chart";
            chart.Title.TextFont.Name = "Arial";
            chart.Title.TextFont.Size = 14;
            chart.Title.TextFont.IsBold = true;
            chart.Title.TextFont.Color = System.Drawing.Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartTitleFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


