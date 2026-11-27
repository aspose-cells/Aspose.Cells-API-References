---
title: "Series.XValuesFormatCode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Representerar formatkoden för X‑värdenas NumberList"
type: docs
url: /sv/net/aspose.cells.charts/series/xvaluesformatcode/
---
## Series.XValuesFormatCode property

Representerar formatkoden för X Values' NumberList.

```csharp
public string XValuesFormatCode { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(200);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Ställ in XValues‑formatkoden
            chart.NSeries[0].XValuesFormatCode = "M/d/yyyy";

            // Spara arbetsboken
            workbook.Save("SeriesPropertyXValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


