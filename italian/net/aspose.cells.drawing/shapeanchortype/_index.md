---
title: "Enum ShapeAnchorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.ShapeAnchorType. Rappresenta il tipo di ancoraggio"
type: docs
url: /it/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Rappresenta il tipo di ancoraggio.

```csharp
public enum ShapeAnchorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| TwoCellAnchor | `0` | Rappresenta un segnaposto di ancoraggio a due celle |
| OneCellAnchor | `1` | Rappresenta un segnaposto di ancoraggio a una cella |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di gruppo
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // Dimostra l'uso di ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Salva la cartella di lavoro
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


