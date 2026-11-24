---
title: "ChartTextFrame.IsAutoText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Eigenschaft. Gibt an, dass der Text automatisch erzeugt wird"
type: docs
url: /de/net/aspose.cells.charts/charttextframe/isautotext/
---
## ChartTextFrame.IsAutoText property

Gibt an, dass der Text automatisch generiert wird.

```csharp
public virtual bool IsAutoText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsAutoTextDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdaten festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagrammtitel konfigurieren
            Aspose.Cells.Charts.ChartTextFrame title = chart.Title;
            title.Text = "Custom Chart Title";
            
            // Demonstriere die IsAutoText-Eigenschaft
            title.IsAutoText = false; // Disable auto-generated text
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartTextFrame_IsAutoText_Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


