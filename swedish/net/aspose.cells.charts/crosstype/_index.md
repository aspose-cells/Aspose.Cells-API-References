---
title: "Enum CrossType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.CrossType enum. Representerar axelns korsningstyp"
type: docs
url: /sv/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Representerar axelkorsningstypen.

```csharp
public enum CrossType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel anger axelns korsningspunkt. |
| Maximum | `1` | Axeln korsar vid det maximala värdet. |
| Minimum | `2` | Axeln korsar vid det minsta värdet. |
| Custom | `3` | Axeln korsar vid det anpassade värdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Lägger till ett nytt kalkylblad i Excel-objektet
            int sheetIndex = workbook.Worksheets.Add();
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            // Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);

            // Ange det maximala värdet för värdeaxeln
            chart.ValueAxis.MaxValue = 200;
            // Ange det minsta värdet för värdeaxeln
            chart.ValueAxis.MinValue = 0;
            // Ange huvudenheten
            chart.ValueAxis.MajorUnit = 25;

            // Category(X) axis korsar vid det maximala värdet
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Ange antalet kategorier eller serier mellan tick‑mark‑etiketterna
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Sparar Excel-filen
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


