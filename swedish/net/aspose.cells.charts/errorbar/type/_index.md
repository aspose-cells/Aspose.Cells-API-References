---
title: "ErrorBar.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorBar-egenskap. Representerar typ av felstapelmängd"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Representerar felstapels mängdtyp.

```csharp
public ErrorBarType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Lägg till exempeldata
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Skapa ett diagram
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Lägg till seriedata
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Ställ in anpassad felstapeltyp och värden
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Spara arbetsboken
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


