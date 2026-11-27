---
title: "Enum ErrorBarType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ErrorBarType-enum. Representerar typ av felstapelförhållande"
type: docs
url: /sv/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

Representerar felstapels mängdtyp.

```csharp
public enum ErrorBarType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Custom | `0` | InnerCustom värdetyp. |
| FixedValue | `1` | Fast värdetyp. |
| Percent | `2` | Procenttyp |
| StDev | `3` | Standardavvikelsetyp. |
| StError | `4` | Standardfeltyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Lägg till lite exempeldata
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Ange felstapelsegenskaper för varje serie i diagrammet
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Spara arbetsboken
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


