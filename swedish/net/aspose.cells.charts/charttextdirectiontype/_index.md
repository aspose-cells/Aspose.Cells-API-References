---
title: "Enum ChartTextDirectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartTextDirectionType enum. Representerar diagrammets textinriktnings typ"
type: docs
url: /sv/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

Representerar textorienteringstypen för diagrammet.

```csharp
public enum ChartTextDirectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Horizontal | `0` | Horisontell riktningstyp. |
| Vertical | `1` | Vertikal riktningstyp. |
| Rotate90 | `2` | Rotera med en nittiograders vinkel. |
| Rotate270 | `3` | Rotera med 270-graders vinkel. |
| Stacked | `4` | Staplad text. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
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
            
            // Lägg till dataserier i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ange diagrammets titel
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // Ställ in textens riktning för diagramrubriken
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // Ställ in textens riktning för kategoriaxelns rubrik
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Ställ in textens riktning för värdeaxelns rubrik
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // Spara arbetsboken
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


