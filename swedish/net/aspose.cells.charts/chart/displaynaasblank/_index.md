---
title: "Chart.DisplayNaAsBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Anger om N/A ska visas som ett tomt värde"
type: docs
url: /sv/net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

Anger om #N/A ska visas som ett tomt värde.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDisplayNaAsBlankDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med några NA‑värden
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(double.NaN); // NA value
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange egenskapen DisplayNaAsBlank
            chart.DisplayNaAsBlank = true;

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Verifiera egenskapen
            Console.WriteLine("DisplayNaAsBlank is set to: " + chart.DisplayNaAsBlank);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


