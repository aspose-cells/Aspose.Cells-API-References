---
title: "ErrorBar.DisplayType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorBar-egenskap. Representerar visningstypen för felstapeln"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Representerar visningstypen för felstapeln.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyDisplayTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Ställ in felstapels visningstyp
            chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;

            // Spara arbetsboken
            workbook.Save("ErrorBarDisplayTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


