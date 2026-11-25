---
title: "Enum MirrorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.MirrorType. Rappresenta il tipo di specchio del riempimento a trama"
type: docs
url: /it/net/aspose.cells.drawing/mirrortype/
---
## MirrorType enumeration

Rappresenta il tipo di specchio del riempimento texture

```csharp
public enum MirrorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuno |
| Horizonal | `1` | Orizzontale |
| Vertical | `2` | Verticale |
| Both | `3` | Entrambi |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMirrorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare MirrorType
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);

            // Imposta il riempimento a trama con diversi tipi di specchio
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
            shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
            shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
            shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;

            // Salva il risultato
            workbook.Save("MirrorTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


