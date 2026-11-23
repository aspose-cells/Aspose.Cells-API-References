---
title: "ShapeTextAlignment.BottomMarginPt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Retourne la marge inférieure en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/
---
## ShapeTextAlignment.BottomMarginPt property

Renvoie la marge inférieure en unités de points

```csharp
public double BottomMarginPt { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyBottomMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "Sample Text";
            
            shape.TextBody.TextAlignment.BottomMarginPt = 2.0d;
            
            Console.WriteLine("Bottom margin set to: " + shape.TextBody.TextAlignment.BottomMarginPt + " points");
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


