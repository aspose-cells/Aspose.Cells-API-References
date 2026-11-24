---
title: "DataLabels.IsAutoText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt an, dass der Text automatisch generiert wird"
type: docs
url: /de/net/aspose.cells.charts/datalabels/isautotext/
---
## DataLabels.IsAutoText property

Gibt an, dass der Text automatisch generiert wird.

```csharp
public override bool IsAutoText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsAutoTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
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
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            foreach (Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
                
                // Demonstriere die IsAutoText-Eigenschaft
                foreach (ChartPoint point in series.Points)
                {
                    Console.WriteLine("IsAutoText before setting: " + point.DataLabels.IsAutoText);
                    point.DataLabels.IsAutoText = false;
                    point.DataLabels.Text = "Custom " + point.YValue;
                    Console.WriteLine("IsAutoText after setting: " + point.DataLabels.IsAutoText);
                    Console.WriteLine("DataLabel Text: " + point.DataLabels.Text);
                }
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsIsAutoTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


