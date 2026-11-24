---
title: "Enum FillPattern"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.FillPattern enum. Enumeriert Typen von Formfüllmustern"
type: docs
url: /de/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Enumeriert Formfüllmuster‑Typen.

```csharp
public enum FillPattern
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Stellt keinen Hintergrund dar. |
| Solid | `1` | Stellt ein einfarbiges Muster dar. |
| Gray5 | `2` | Stellt ein 5 % Graumuster dar. |
| Gray10 | `3` | Stellt ein 10 % Graumuster dar. |
| Gray20 | `4` | Stellt ein 20 % Graumuster dar. |
| Gray30 | `5` | Stellt ein 30 % Graumuster dar. |
| Gray40 | `6` | Stellt ein 40 % Graumuster dar. |
| Gray50 | `7` | Stellt ein 50% Graumuster dar. |
| Gray60 | `8` | Stellt ein 60 % Graumuster dar. |
| Gray70 | `9` | Stellt ein 70 % Graumuster dar. |
| Gray75 | `10` | Stellt ein 75% Graumuster dar. |
| Gray80 | `11` | Stellt ein 80 % Graumuster dar. |
| Gray90 | `12` | Stellt ein 90 % Graumuster dar. |
| Gray25 | `13` | Stellt ein 25% Graumuster dar. |
| LightDownwardDiagonal | `14` | Stellt ein leichtes nach unten diagonales Muster dar. |
| LightUpwardDiagonal | `15` | Stellt ein leichtes nach oben diagonales Muster dar. |
| DarkDownwardDiagonal | `16` | Stellt ein dunkles nach unten diagonales Muster dar. |
| DarkUpwardDiagonal | `17` | Stellt ein dunkles nach oben diagonales Muster dar. |
| WideDownwardDiagonal | `18` | Stellt ein breites nach unten diagonales Muster dar. |
| WideUpwardDiagonal | `19` | Stellt ein breites nach oben diagonales Muster dar. |
| LightVertical | `20` | Stellt ein leichtes vertikales Muster dar. |
| LightHorizontal | `21` | Stellt ein leichtes horizontales Muster dar. |
| NarrowVertical | `22` | Stellt ein schmales vertikales Muster dar. |
| NarrowHorizontal | `23` | Stellt ein schmales horizontales Muster dar. |
| DarkVertical | `24` | Stellt ein dunkles vertikales Muster dar. |
| DarkHorizontal | `25` | Stellt ein dunkles horizontales Muster dar. |
| DashedDownwardDiagonal | `26` | Stellt ein gestricheltes diagonales Muster nach unten dar. |
| DashedUpwardDiagonal | `27` | Stellt ein gestricheltes diagonales Muster nach oben dar. |
| DashedVertical | `28` | Stellt ein gestricheltes vertikales Muster dar. |
| DashedHorizontal | `29` | Stellt ein gestricheltes horizontales Muster dar. |
| SmallConfetti | `30` | Stellt ein kleines Konfetti-Muster dar. |
| LargeConfetti | `31` | Stellt ein großes Konfetti-Muster dar. |
| ZigZag | `32` | Stellt ein Zickzack-Muster dar. |
| Wave | `33` | Stellt ein Wellenmuster dar. |
| DiagonalBrick | `34` | Stellt ein diagonales Ziegelmuster dar. |
| HorizontalBrick | `35` | Stellt ein horizontales Ziegelmuster dar. |
| Weave | `36` | Stellt ein Webmuster dar. |
| Plaid | `37` | Stellt ein Karomuster dar. |
| Divot | `38` | Stellt ein Vertiefungsmuster dar. |
| DottedGrid | `39` | Stellt ein gepunktetes Rastermuster dar. |
| DottedDiamond | `40` | Stellt ein gepunktetes Rautenmuster dar. |
| Shingle | `41` | Stellt ein Schindelmuster dar. |
| Trellis | `42` | Stellt ein Rankgittermuster dar. |
| Sphere | `43` | Stellt ein Kugelmuster dar. |
| SmallGrid | `44` | Stellt ein kleines Rastermuster dar. |
| LargeGrid | `45` | Stellt ein großes Rastermuster dar. |
| SmallCheckerBoard | `46` | Stellt ein kleines Schachbrettmuster dar. |
| LargeCheckerBoard | `47` | Stellt ein großes Schachbrettmuster dar. |
| OutlinedDiamond | `48` | Stellt ein umrandetes Rautenmuster dar. |
| SolidDiamond | `49` | Stellt ein solides Rautenmuster dar. |
| Unknown | `50` | Stellt ein unbekanntes Muster dar. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Füllmuster für die erste Serie festlegen
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Speichere die Arbeitsmappe
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


