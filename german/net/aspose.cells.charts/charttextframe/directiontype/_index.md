---
title: "ChartTextFrame.DirectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartTextFrame-Eigenschaft. Gibt die Richtung des Textes zurück und legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Liest und legt die Textausrichtung fest.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // Das Hinzufügen eines Arbeitsblatts gibt dessen Index zurück, anschließend rufen wir das Arbeitsblatt über den Index ab.
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Zugriff auf und Konfiguration des Titels
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // Demonstrieren Sie die DirectionType‑Eigenschaft
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


