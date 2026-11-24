---
title: "DataLabels.NumberFormatLinked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Wahr, wenn das Zahlenformat mit den Zellen verknüpft ist, sodass sich das Zahlenformat in den Beschriftungen ändert, wenn es sich in den Zellen ändert."
type: docs
url: /de/net/aspose.cells.charts/datalabels/numberformatlinked/
---
## DataLabels.NumberFormatLinked property

True, wenn das Zahlenformat mit den Zellen verknüpft ist (so dass sich das Zahlenformat in den Beschriftungen ändert, wenn es sich in den Zellen ändert).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Formatted Value");
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie hinzufügen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Datenbeschriftungen konfigurieren
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.NumberFormatLinked = true; // Link number format from source cells
            
            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsNumberFormatLinkedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


