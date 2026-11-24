---
title: "TickLabels.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Gibt ein Font-Objekt zurück, das die Schriftart des angegebenen TickLabels-Objekts darstellt."
type: docs
url: /de/net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Gibt ein `Font`-Objekt zurück, das die Schriftart des angegebenen TickLabels-Objekts darstellt.

```csharp
public Font Font { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "A1:A1";
            
            // Zugriff auf die Schriftart der TickLabels
            Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
            Font font = tickLabels.Font;
            
            // Setze Schriftarteigenschaften
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsFontDemo.xlsx");
            
            Console.WriteLine("TickLabels font properties set successfully.");
        }
    }
}
```

### Siehe auch

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


