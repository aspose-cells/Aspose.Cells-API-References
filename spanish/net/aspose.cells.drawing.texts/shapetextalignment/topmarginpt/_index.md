---
title: "ShapeTextAlignment.TopMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Devuelve el margen superior en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/topmarginpt/
---
## ShapeTextAlignment.TopMarginPt property

Devuelve el margen superior en unidades de puntos

```csharp
public double TopMarginPt { get; set; }
```

### Ejemplos

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

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


