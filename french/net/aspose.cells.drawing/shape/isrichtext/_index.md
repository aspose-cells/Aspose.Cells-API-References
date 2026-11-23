---
title: "Shape.IsRichText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si le texte est enrichi ou non"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Indique si le texte est du texte enrichi.

```csharp
public bool IsRichText { get; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme avec du texte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Vérifiez si le texte est enrichi
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

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


