---
title: "Shape.TextHorizontalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di allineamento orizzontale del testo della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/texthorizontalalignment/
---
## Shape.TextHorizontalAlignment property

Ottiene e imposta il tipo di allineamento orizzontale del testo della forma.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Imposta il testo e l'allineamento
            shape.Text = "Sample Text";
            shape.TextHorizontalAlignment = TextAlignmentType.Center;

            // Cambia l'allineamento se attualmente è in basso
            if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextHorizontalAlignment = TextAlignmentType.Center;
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextAlignmentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


