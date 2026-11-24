---
title: "DataLabels.ShowCellRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt an, ob der Zellbereich als Datenbeschriftungen angezeigt werden soll"
type: docs
url: /de/net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Gibt an, ob der Zellbereich als Datenlabels angezeigt werden soll.

```csharp
public bool ShowCellRange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCellRangeDemo
    {
        public static void Run()
        {
            // Arbeitsmappe erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Datenbeschriftungen mit ShowCellRange konfigurieren
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCellRange = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.Font.Color = Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


