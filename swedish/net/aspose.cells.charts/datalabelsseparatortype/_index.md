---
title: "Enum DataLabelsSeparatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.DataLabelsSeparatorType enum. Representerar separatortypen för DataLabels"
type: docs
url: /sv/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

Representerar separator‑typen för DataLabels.

```csharp
public enum DataLabelsSeparatorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Auto | `0` | Representerar automatisk separator |
| Space | `1` | Representerar mellanslag(" ") |
| Comma | `2` | Representerar komma(",") |
| Semicolon | `3` | Representerar ett semikolon(";") |
| Period | `4` | Representerar punkt(".") |
| NewLine | `5` | Representerar ny rad("\n") |
| Custom | `6` | Representerar anpassad separator |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för diagrammet
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till dataserien i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Få åtkomst till dataetiketterna för den första serien
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Ställ in separatortypen till komma
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Aktivera dataetiketter och ställ in några egenskaper
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Ställ in teckensnittsegenskaper
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Spara arbetsboken
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


