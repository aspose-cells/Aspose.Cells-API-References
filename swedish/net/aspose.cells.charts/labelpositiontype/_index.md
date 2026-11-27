---
title: "Enum LabelPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.LabelPositionType enum. Representerar datalabelens positionstyp"
type: docs
url: /sv/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Representerar datalabelns positionstyp.

```csharp
public enum LabelPositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Center | `0` | Gäller endast för stapel- och 2D/3D-cirkeldiagram |
| InsideBase | `1` | Gäller endast för stapel- och 2D/3D-cirkeldiagram |
| InsideEnd | `2` | Gäller endast för stapeldiagram |
| OutsideEnd | `3` | Gäller endast för stapel- och 2D/3D-cirkeldiagram |
| Above | `4` | Gäller endast för linjediagram |
| Below | `5` | Gäller endast för linjediagram |
| Left | `6` | Gäller endast för linjediagram |
| Right | `7` | Gäller endast för linjediagram |
| BestFit | `8` | Gäller endast för 2D/3D-pi-diagram |
| Moved | `9` | Användaren flyttade datamärkningarna. Detta är endast för att läsa diagrammet från mallfilen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till dataserien i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Få åtkomst till dataetiketterna för den första serien
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Ställ in positionen för datamärkningarna
            dataLabels.Position = LabelPositionType.InsideBase;

            // Visa kategorinamnet i datamärkningarna
            dataLabels.ShowCategoryName = true;

            // Visa värdet i datamärkningarna
            dataLabels.ShowValue = true;

            // Spara arbetsboken
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


