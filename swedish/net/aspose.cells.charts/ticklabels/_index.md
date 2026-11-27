---
title: "Klass TickLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.TickLabels-klass. Representerar tickmark-etiketterna som är associerade med tickmarkeringar på ett diagramaxel"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Representerar tick‑markeringsetiketter som är associerade med tick‑markeringar på en diagramaxel.

```csharp
public class TickLabels
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Hämtar och anger textjusteringen för ticketiketterna på axeln. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Hämtar och anger visningsläget för bakgrunden |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Hämtar och anger textens riktning. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Hämtar och anger visningsformatet för siffror för ticketiketterna. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Returnerar ett [`Font`](./font/)‑objekt som representerar teckensnittet för det angivna TickLabels‑objektet. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Indikerar om rotationsvinkeln är automatisk |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Representerar formatnumret för TickLabels‑objektet. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Representerar formatsträngen för TickLabels‑objektet. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Hämtar och anger avståndet för etiketter från kategoriaxeln. Detta gäller endast kategori‑(x‑)axeln. |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Representerar textens läsriktning. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Representerar textens rotationsvinkel medurs. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Representerar läsriktning för text. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Hämtar de visade ticketiketterna för axeln. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);

            // Åtkomst till värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Åtkomst till ticketiketterna på värdeaxeln
            TickLabels tickLabels = valueAxis.TickLabels;

            // Ställ in egenskaper för ticketiketterna
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Spara arbetsboken
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


