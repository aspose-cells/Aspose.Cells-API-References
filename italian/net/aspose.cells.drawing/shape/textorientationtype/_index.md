---
title: "Shape.TextOrientationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta il tipo di orientamento del testo della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Ottiene e imposta il tipo di orientamento del testo della forma.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Imposta il testo per la forma
            shape.Text = "Sample Text";

            // Verifica e modifica l'orientamento del testo
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


