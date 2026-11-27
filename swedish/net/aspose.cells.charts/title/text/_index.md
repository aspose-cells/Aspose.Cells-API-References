---
title: "Title.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Title-egenskapen. Hämtar eller anger texten för visningsenhetens etikett"
type: docs
url: /sv/net/aspose.cells.charts/title/text/
---
## Title.Text property

Hämtar eller anger texten för displayenhetsetiketten.

```csharp
public override string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);
            
            // Lägg till ett diagram och ange dess ValueAxis‑titels text
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.ValueAxis.Title.Text = "Sales Amount";
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


