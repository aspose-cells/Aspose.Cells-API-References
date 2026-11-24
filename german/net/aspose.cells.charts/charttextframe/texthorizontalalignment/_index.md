---
title: "ChartTextFrame.TextHorizontalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Eigenschaft. Gibt die horizontale Textausrichtung zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

Liest und legt die horizontale Ausrichtung des Textes fest.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Fügen Sie ein Diagramm hinzu und setzen Sie dessen Datenbereich
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hole den Diagrammtitel und setze Eigenschaften
            Title title = chart.Title;
            title.Text = "Sample Chart Title";
            
            // Demonstriere die TextHorizontalAlignment-Eigenschaft
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            Console.WriteLine("Title horizontal alignment set to: " + title.TextHorizontalAlignment);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartTextHorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


