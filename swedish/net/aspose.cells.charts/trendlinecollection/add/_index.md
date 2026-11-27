---
title: "TrendlineCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TrendlineCollection‑metod. Lägger till ett Trendline‑objekt i den här samlingen med den angivna typen"
type: docs
url: /sv/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Lägger till ett [`Trendline`](../../trendline/)‑objekt i den här samlingen med den angivna typen.

```csharp
public int Add(TrendlineType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | TrendlineType | Trendline‑typ. |

### Returvärde

[`Trendline`](../../trendline/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till seriedata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Lägg till exponentiell trendlinje till den första serien
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // Spara arbetsboken
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Lägger till ett [`Trendline`](../../trendline/)‑objekt i den här samlingen med angiven typ och namn.

```csharp
public int Add(TrendlineType type, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | TrendlineType | Trendline‑typ. |
| namn | String | Trendline‑namn. |

### Returvärde

[`Trendline`](../../trendline/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Lägg till serie och ange data
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // Lägg till trendlinje med TrendlineType och namn
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // Ställ in några trendline‑egenskaper
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


