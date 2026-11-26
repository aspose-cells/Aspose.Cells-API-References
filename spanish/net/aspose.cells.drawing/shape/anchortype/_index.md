---
title: "Shape.AnchorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el tipo del marcador de posición de anclaje de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Obtiene y establece el tipo del marcador de posición del ancla de forma.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma con el tipo de anclaje predeterminado
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Verifica y modifica el tipo de anclaje
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


