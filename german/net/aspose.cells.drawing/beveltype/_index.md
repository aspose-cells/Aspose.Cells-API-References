---
title: "Enum BevelType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.BevelType‑Enum. Stellt eine Voreinstellung für einen Typ von Abschrägung dar, die auf eine Form in 3D angewendet werden kann."
type: docs
url: /de/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

Stellt eine Voreinstellung für einen Abschrägungs‑Typ dar, die auf eine Form in 3D angewendet werden kann.

```csharp
public enum BevelType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine Abschrägung |
| Angle | `1` | Winkel |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Kreis |
| Convex | `4` | Konvex |
| CoolSlant | `5` | Coole Schräge |
| Cross | `6` | Kreuz |
| Divot | `7` | Kerbe |
| HardEdge | `8` | Harte Kante |
| RelaxedInset | `9` | Entspannte Einrückung |
| Riblet | `10` | Rippe |
| Slope | `11` | Steigung |
| SoftRound | `12` | Weiche Rundung |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class BevelTypeDemo
    {
        public static void BevelTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Greife auf das 3D-Format der Form zu
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Setze den oberen Abschrägungstyp und die Abmessungen
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Setze den unteren Abschrägungstyp und die Abmessungen
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Speichere die Arbeitsmappe
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


