---
title: "ShapeTextAlignment.TopMarginPt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Retourne la marge supérieure en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/topmarginpt/
---
## ShapeTextAlignment.TopMarginPt property

Renvoie la marge supérieure en unités de points

```csharp
public double TopMarginPt { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Text = "Sample Text";
            
            shape.TextBody.TextAlignment.TopMarginPt = 2.0d;
            
            workbook.Save("ShapeTextAlignmentTopMarginPtDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


