---
title: "ShapeTextAlignment.TextShapeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Gibt den Transformations-Typ des Textes zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/textshapetype/
---
## ShapeTextAlignment.TextShapeType property

Liest und setzt den Transformationstyp des Textes.

```csharp
public AutoShapeType TextShapeType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextShapeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Textfeldform hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);

            // Erhalte die Textausrichtung der Form
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Setzen Sie die TextShapeType-Eigenschaft
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;

            // Speichere die Arbeitsmappe
            workbook.Save("TextShapeTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [AutoShapeType](../../../aspose.cells.drawing/autoshapetype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


