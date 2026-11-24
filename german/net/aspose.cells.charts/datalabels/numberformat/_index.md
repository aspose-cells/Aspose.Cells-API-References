---
title: "DataLabels.NumberFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Stellt die Formatzeichenfolge für das DataLabels-Objekt dar"
type: docs
url: /de/net/aspose.cells.charts/datalabels/numberformat/
---
## DataLabels.NumberFormat property

Stellt die Formatzeichenfolge für das DataLabels-Objekt dar.

```csharp
public string NumberFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberFormatDemo
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
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Benutzerdefiniertes Zahlenformat für Datenbeschriftungen festlegen
            series.DataLabels.NumberFormat = "_(* #,##0_);_(* \\(#,##0\\);_(* \"-\"??_);_(@_)";
            
            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


