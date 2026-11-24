---
title: "Area.Formatting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Area-Eigenschaft. Stellt die Formatierung des Bereichs dar"
type: docs
url: /de/net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Stellt die Formatierung des Bereichs dar.

```csharp
public FormattingType Formatting { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFormattingDemo
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
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Auf den Diagrammbereich zugreifen und Formatierung festlegen
            ChartArea chartArea = chart.ChartArea;
            chartArea.Area.Formatting = FormattingType.None;

            // Speichere die Arbeitsmappe
            workbook.Save("AreaPropertyFormattingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


