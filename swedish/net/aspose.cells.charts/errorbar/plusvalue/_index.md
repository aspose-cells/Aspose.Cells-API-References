---
title: "ErrorBar.PlusValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorBar-egenskap. Representerar positiv felmängd när felstapeln är av typen Anpassad"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/plusvalue/
---
## ErrorBar.PlusValue property

Representerar positivt felvärde när felstapeln är Custom.

```csharp
public string PlusValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyPlusValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);

            // Konfigurera felstaplar
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";  // Using PlusValue property
            errorBar.MinusValue = "=A3";

            // Spara arbetsboken
            workbook.Save("ErrorBarPlusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


