---
title: "ShapeTextAlignment.IsTextWrapped"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Ruft den Zeilenumbruchtyp der Form, die Text enthält, ab oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/istextwrapped/
---
## ShapeTextAlignment.IsTextWrapped property

Liest oder setzt den Zeilenumbruchtyp des Shapes, das Text enthält.

```csharp
public bool IsTextWrapped { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Formtext festlegen
            shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";

            // Rufen Sie die Textausrichtung ab und setzen Sie IsTextWrapped
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.IsTextWrapped = true;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


