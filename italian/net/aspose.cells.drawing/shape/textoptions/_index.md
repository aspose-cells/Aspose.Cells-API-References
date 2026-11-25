---
title: "Shape.TextOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Rappresenta le opzioni di testo della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/textoptions/
---
## Shape.TextOptions property

Rappresenta le opzioni di testo della forma.

```csharp
public TextOptions TextOptions { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Imposta il testo per la forma
            shape.Text = "Sample Text";

            // Accedi e modifica TextOptions
            TextOptions opt = shape.TextOptions;
            opt.Color = Color.Blue;
            opt.Size = 8;

            // Salva la cartella di lavoro
            workbook.Save("ShapeTextOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


