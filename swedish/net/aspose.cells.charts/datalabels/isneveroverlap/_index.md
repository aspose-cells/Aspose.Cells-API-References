---
title: "DataLabels.IsNeverOverlap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Anger om dataetiketter aldrig överlappar när en pajdiagram konverteras till bild. Observera att denna egenskap endast är meningsfull när ett pajdiagram konverteras till bild"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/isneveroverlap/
---
## DataLabels.IsNeverOverlap property

Indikerar om Datalabels aldrig överlappar när en pajdiagram konverteras till bild. Obs: den här egenskapen är endast meningsfull när en pajdiagram konverteras till bild.

```csharp
public bool IsNeverOverlap { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsNeverOverlapDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datamärkningar
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Hämta dataetiketter och sätt IsNeverOverlap-egenskapen
            DataLabels dataLabels = series.DataLabels;
            Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
            
            // Sätt IsNeverOverlap till sant
            dataLabels.IsNeverOverlap = true;
            Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);

            // Spara arbetsboken
            workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


