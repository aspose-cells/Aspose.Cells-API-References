---
title: "ShapeTextAlignment.IsAutoMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Indica si el margen del marco de texto es automático"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/isautomargin/
---
## ShapeTextAlignment.IsAutoMargin property

Indica si el margen del marco de texto es automático.

```csharp
public bool IsAutoMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsAutoMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Acceder a la alineación de texto y establecer IsAutoMargin
            shape.TextBody.TextAlignment.IsAutoMargin = true;

            // Establecer algún texto para demostrar
            shape.Text = "Sample text with auto margins";

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


