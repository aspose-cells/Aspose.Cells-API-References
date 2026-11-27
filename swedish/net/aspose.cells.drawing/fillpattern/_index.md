---
title: "Enum FillPattern"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.FillPattern enum. Enumererar typer av fyllningsmönster för former"
type: docs
url: /sv/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Enumererar typer av formfyllningsmönster.

```csharp
public enum FillPattern
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Representerar ingen bakgrund. |
| Solid | `1` | Representerar solid mönster. |
| Gray5 | `2` | Representerar 5 % grått mönster. |
| Gray10 | `3` | Representerar 10 % grått mönster. |
| Gray20 | `4` | Representerar 20 % grått mönster. |
| Gray30 | `5` | Representerar 30 % grått mönster. |
| Gray40 | `6` | Representerar 40 % grått mönster. |
| Gray50 | `7` | Representerar 50 % grått mönster. |
| Gray60 | `8` | Representerar 60 % grått mönster. |
| Gray70 | `9` | Representerar 70 % grått mönster. |
| Gray75 | `10` | Representerar 75 % grått mönster. |
| Gray80 | `11` | Representerar 80 % grått mönster. |
| Gray90 | `12` | Representerar 90 % grått mönster. |
| Gray25 | `13` | Representerar 25 % grått mönster. |
| LightDownwardDiagonal | `14` | Representerar ljust nedåtriktat diagonalt mönster. |
| LightUpwardDiagonal | `15` | Representerar ljust uppåtriktat diagonalt mönster. |
| DarkDownwardDiagonal | `16` | Representerar mörkt nedåtriktat diagonalt mönster. |
| DarkUpwardDiagonal | `17` | Representerar mörkt uppåtriktat diagonalt mönster. |
| WideDownwardDiagonal | `18` | Representerar brett nedåtriktat diagonalt mönster. |
| WideUpwardDiagonal | `19` | Representerar brett uppåtriktat diagonalt mönster. |
| LightVertical | `20` | Representerar ljust vertikalt mönster. |
| LightHorizontal | `21` | Representerar ljust horisontellt mönster. |
| NarrowVertical | `22` | Representerar smalt vertikalt mönster. |
| NarrowHorizontal | `23` | Representerar smalt horisontellt mönster. |
| DarkVertical | `24` | Representerar mörkt vertikalt mönster. |
| DarkHorizontal | `25` | Representerar mörkt horisontellt mönster. |
| DashedDownwardDiagonal | `26` | Representerar streckat nedåtriktat diagonalt mönster. |
| DashedUpwardDiagonal | `27` | Representerar streckat uppåtriktat diagonalt mönster. |
| DashedVertical | `28` | Representerar streckat vertikalt mönster. |
| DashedHorizontal | `29` | Representerar streckat horisontellt mönster. |
| SmallConfetti | `30` | Representerar litet konfettimönster. |
| LargeConfetti | `31` | Representerar stort konfettimönster. |
| ZigZag | `32` | Representerar sicksackmönster. |
| Wave | `33` | Representerar vågmönster. |
| DiagonalBrick | `34` | Representerar diagonal tegelmönster. |
| HorizontalBrick | `35` | Representerar horisontellt tegelmönster. |
| Weave | `36` | Representerar vävmönster. |
| Plaid | `37` | Representerar rutigt mönster. |
| Divot | `38` | Representerar gropmönster. |
| DottedGrid | `39` | Representerar prickigt rutnätmönster. |
| DottedDiamond | `40` | Representerar prickig diamantmönster. |
| Shingle | `41` | Representerar takpannemönster. |
| Trellis | `42` | Representerar gallermönster. |
| Sphere | `43` | Representerar sfärmönster. |
| SmallGrid | `44` | Representerar litet rutnätmönster. |
| LargeGrid | `45` | Representerar stort rutnätmönster. |
| SmallCheckerBoard | `46` | Representerar litet schackbrädemönster. |
| LargeCheckerBoard | `47` | Representerar stort schackbrädemönster. |
| OutlinedDiamond | `48` | Representerar ett konturerat diamantmönster. |
| SolidDiamond | `49` | Representerar ett fyllt diamantmönster. |
| Unknown | `50` | Representerar ett okänt mönster. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange fyllningsmönster för den första serien
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Spara arbetsboken
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


