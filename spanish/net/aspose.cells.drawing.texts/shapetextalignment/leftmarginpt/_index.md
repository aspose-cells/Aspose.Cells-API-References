---
title: "ShapeTextAlignment.LeftMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Devuelve el margen izquierdo en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/
---
## ShapeTextAlignment.LeftMarginPt property

Devuelve el margen izquierdo en unidades de puntos

```csharp
public double LeftMarginPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            // Establecer texto para la forma
            shape.Text = "Sample text with left margin";

            // Acceder a la alineación de texto y establecer el margen izquierdo en puntos
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.LeftMarginPt = 2.0d;

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextAlignmentLeftMarginPtDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


