---
title: "Title.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Title property. Gibt den Text der Anzeigeeinheitenbeschriftung zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.charts/title/text/
---
## Title.Text property

Liest oder schreibt den Text der Anzeigeeinheitenbeschriftung.

```csharp
public override string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);
            
            // Fügen Sie ein Diagramm hinzu und setzen Sie den Titeltext der ValueAxis.
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.ValueAxis.Title.Text = "Sales Amount";
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


