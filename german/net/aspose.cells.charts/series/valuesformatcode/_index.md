---
title: "Series.ValuesFormatCode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Stellt den Formatcode der Values NumberList dar."
type: docs
url: /de/net/aspose.cells.charts/series/valuesformatcode/
---
## Series.ValuesFormatCode property

Stellt den Formatcode der Werte‑NumberList dar.

```csharp
public string ValuesFormatCode { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesFormatCodeDemo
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
            worksheet.Cells["B2"].PutValue(0.25);
            worksheet.Cells["B3"].PutValue(0.5);
            worksheet.Cells["B4"].PutValue(0.75);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze den Werteformatcode für die erste Series
            chart.NSeries[0].ValuesFormatCode = "0.00%";

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertyValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


