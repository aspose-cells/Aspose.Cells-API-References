---
title: "Enum ErrorBarDisplayType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ErrorBarDisplayType enum. Representerar felstapels visningstyp"
type: docs
url: /sv/net/aspose.cells.charts/errorbardisplaytype/
---
## ErrorBarDisplayType enumeration

Representerar felstapels visningstyp.

```csharp
public enum ErrorBarDisplayType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Both | `0` | Båda |
| Minus | `1` | Minus |
| None | `2` | Ingen |
| Plus | `3` | Plus |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDisplayTypeDemo
    {
        public static void ErrorBarDisplayTypeExample()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue(2);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(6);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(7);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Lägg till ett stapeldiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Konfigurera felstaplar för varje serie i diagrammet
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Spara arbetsboken
            workbook.Save("ErrorBarDisplayTypeExample.xlsx");
            workbook.Save("ErrorBarDisplayTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


