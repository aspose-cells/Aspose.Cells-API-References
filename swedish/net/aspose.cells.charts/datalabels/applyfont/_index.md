---
title: "DataLabels.ApplyFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-metod. Applicera teckensnittet för dataetiketterna på alla undernoder"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

Applicera teckensnittet för dataetiketterna på alla underordnade noder.

```csharp
public void ApplyFont()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Visa dataetiketter
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Ange ny teckensnittsfärg för dataetiketter
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // Applicera teckensnittinställningarna på alla dataetiketter
            series.DataLabels.ApplyFont();
            
            // Spara arbetsboken
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


