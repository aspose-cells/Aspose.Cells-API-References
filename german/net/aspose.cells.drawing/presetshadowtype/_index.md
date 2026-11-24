---
title: "Enum PresetShadowType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PresetShadowType-Enum. Stellt einen vordefinierten Schattentyp dar"
type: docs
url: /de/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Stellt den voreingestellten Schatten‑Typ dar.

```csharp
public enum PresetShadowType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| NoShadow | `0` | Kein Schatten. |
| Custom | `1` | Benutzerdefinierter Schatten. |
| OffsetDiagonalBottomRight | `2` | Außen Schattenversatz diagonal unten rechts. |
| OffsetBottom | `3` | Außen Schattenversatz unten. |
| OffsetDiagonalBottomLeft | `4` | Außen Schattenversatz diagonal unten links. |
| OffsetRight | `5` | Außen Schattenversatz rechts. |
| OffsetCenter | `6` | Außen Schattenversatz Mitte. |
| OffsetLeft | `7` | Außen Schattenversatz links. |
| OffsetDiagonalTopRight | `8` | Außen Schattenversatz diagonal oben rechts. |
| OffsetTop | `9` | Außen Schattenversatz oben. |
| OffsetDiagonalTopLeft | `10` | Außen Schattenversatz diagonal oben links. |
| InsideDiagonalTopLeft | `11` | Innerer Schatten diagonal oben links. |
| InsideTop | `12` | Innerer Schatten oben. |
| InsideDiagonalTopRight | `13` | Innerer Schatten diagonal oben rechts. |
| InsideLeft | `14` | Innerer Schatten links. |
| InsideCenter | `15` | Innerer Schatten Mitte. |
| InsideRight | `16` | Innerer Schatten rechts. |
| InsideDiagonalBottomLeft | `17` | Innerer Schatten diagonal unten links. |
| InsideBottom | `18` | Innerer Schatten unten. |
| InsideDiagonalBottomRight | `19` | Innerer Schatten diagonal unten rechts. |
| PerspectiveDiagonalUpperLeft | `20` | Äußerer Schatten perspektivisch diagonal oben links. |
| PerspectiveDiagonalUpperRight | `21` | Äußerer Schatten perspektivisch diagonal oben rechts. |
| Below | `22` | Äußerer Schatten unten. |
| PerspectiveDiagonalLowerLeft | `23` | Äußerer Schatten perspektivisch diagonal unten links. |
| PerspectiveDiagonalLowerRight | `24` | Äußerer Schatten perspektivisch diagonal unten rechts. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um Schatteneffekte zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Verschiedene voreingestellte Schattenarten festlegen
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Zu einem anderen Schattenstil wechseln
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Speichere die Arbeitsmappe
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


