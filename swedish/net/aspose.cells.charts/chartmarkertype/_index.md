---
title: "Enum ChartMarkerType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartMarkerType enum. Representerar markörstilen i ett linjediagram, spridningsdiagram eller radardiagram"
type: docs
url: /sv/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Representerar markörstilen i ett linjediagram, spridningsdiagram eller radardiagram.

```csharp
public enum ChartMarkerType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Automatiska markörer. |
| Circle | `1` | Cirkulära markörer. |
| Dash | `2` | Långa stapelmarkörer |
| Diamond | `3` | Diamantformade markörer. |
| Dot | `4` | Korta stapelmarkörer. |
| None | `5` | Inga markörer. |
| SquarePlus | `6` | Fyrkantiga markörer med ett plustecken. |
| Square | `7` | Fyrkantiga markörer. |
| SquareStar | `8` | Fyrkantiga markörer med en asterisk. |
| Triangle | `9` | Triangulära markörer. |
| SquareX | `10` | Fyrkantiga markörer med ett X. |
| Picture | `11` | Bild |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till dataserien i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Få åtkomst till markören för den första serien
            Marker marker = chart.NSeries[0].Marker;

            // Ställ in markörstilen
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Ställ in markörstorleken
            marker.MarkerSize = 10;

            // Ställ in markörens förgrunds- och bakgrundsfärger
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


