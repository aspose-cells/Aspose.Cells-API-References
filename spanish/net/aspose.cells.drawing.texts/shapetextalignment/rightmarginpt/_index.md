---
title: "ShapeTextAlignment.RightMarginPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Devuelve el margen derecho en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/
---
## ShapeTextAlignment.RightMarginPt property

Devuelve el margen derecho en unidades de puntos

```csharp
public double RightMarginPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Acceder a la alineación de texto
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Establecer el margen derecho en puntos
            shapeTextAlignment.RightMarginPt = 2.0d;

            // Verificar la propiedad obteniendo el valor de nuevo
            Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


