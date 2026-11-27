---
title: "Enum CategoryType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.CategoryType enum. Representerar kategorialaxeltypen"
type: docs
url: /sv/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

Representerar kategoriaxeltypen.

```csharp
public enum CategoryType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Lägger till ett nytt kalkylblad i Excel-objektet
            int sheetIndex = workbook.Worksheets.Add();
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            // Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("B2:C4", true);

            // Ställer in kategorinamnen för X-axeln från intervallet "A2:A5"
            chart.NSeries[0].XValues = "A2:A4";

            // Ställer in kategorialaxeltypen till TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Ställer in huvudenhetsskalan för kategorialaxeln
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Ställer in mindre enhetsskalan för kategorialaxeln
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Sparar Excel-filen
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


