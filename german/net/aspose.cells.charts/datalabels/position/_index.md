---
title: "DataLabels.Position"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt die Position der Datenbeschriftung an"
type: docs
url: /de/net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Stellt die Position des Datenlabels dar.

```csharp
public LabelPositionType Position { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyPositionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            chart.NSeries[0].DataLabels.ShowValue = true;
            
            // Position der Datenbeschriftung festlegen
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Right;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsPositionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


