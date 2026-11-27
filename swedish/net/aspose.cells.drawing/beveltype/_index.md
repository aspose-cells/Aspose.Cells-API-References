---
title: "Enum BevelType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.BevelType enum. Representerar en förinställning för en typ av avfasning som kan tillämpas på en form i 3D"
type: docs
url: /sv/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

Representerar en förinställning för en typ av fasning som kan tillämpas på en form i 3D.

```csharp
public enum BevelType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen avfasning |
| Angle | `1` | Vinkel |
| ArtDeco | `2` | Art deco |
| Circle | `3` | Cirkel |
| Convex | `4` | Konvex |
| CoolSlant | `5` | Cool lutning |
| Cross | `6` | Kors |
| Divot | `7` | Grop |
| HardEdge | `8` | Hård kant |
| RelaxedInset | `9` | Avslappnad infogning |
| Riblet | `10` | Ribb |
| Slope | `11` | Lutning |
| SoftRound | `12` | Mjuk rundning |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Åtkomst till formens 3D-format
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Ställ in toppens fasningstyp och dimensioner
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Ställ in bottnens fasningstyp och dimensioner
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Spara arbetsboken
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


