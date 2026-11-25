---
title: "Shape.IsRichText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se il testo è rich text."
type: docs
url: /it/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Se il testo è o meno testo ricco.

```csharp
public bool IsRichText { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsRichTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con testo.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Verifica se il testo è rich text.
            if (shape.IsRichText)
            {
                Console.WriteLine("The text is rich text.");
            }
            else
            {
                Console.WriteLine("The text is not rich text.");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


