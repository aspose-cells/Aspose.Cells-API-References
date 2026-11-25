---
title: "Enum BevelType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.BevelType enum. Rappresenta un preset per un tipo di smussatura che può essere applicato a una forma in 3D"
type: docs
url: /it/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

Rappresenta un preset per un tipo di smussatura che può essere applicato a una forma in 3D.

```csharp
public enum BevelType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna smussatura |
| Angle | `1` | Angolo |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Cerchio |
| Convex | `4` | Convesso |
| CoolSlant | `5` | Inclinazione fresca |
| Cross | `6` | Croce |
| Divot | `7` | Incavo |
| HardEdge | `8` | Bordo rigido |
| RelaxedInset | `9` | Inserimento rilassato |
| Riblet | `10` | Ribetto |
| Slope | `11` | Pendenza |
| SoftRound | `12` | Arrotondamento morbido |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Accedi al formato 3D della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Imposta il tipo di smusso superiore e le dimensioni
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Imposta il tipo di smusso inferiore e le dimensioni
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Salva la cartella di lavoro
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


