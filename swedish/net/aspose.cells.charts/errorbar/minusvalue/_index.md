---
title: "ErrorBar.MinusValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorBar-egenskap. Representerar negativ felmängd när felstapeln är av typen Anpassad"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Representerar negativt felvärde när felstapeln är av typen Custom.

```csharp
public string MinusValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyMinusValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(15);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie
            chart.NSeries.Add("B2:B3", true);

            // Konfigurera felstaplar
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";
            errorBar.MinusValue = "=A3";

            // Spara arbetsboken
            workbook.Save("ErrorBarMinusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


