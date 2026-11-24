---
title: "Shape.IsRichText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, ob der Text Rich Text ist oder nicht."
type: docs
url: /de/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Ob der Text Rich Text ist oder nicht.

```csharp
public bool IsRichText { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Form mit Text hinzu.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Überprüfen Sie, ob der Text Rich Text ist.
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

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


