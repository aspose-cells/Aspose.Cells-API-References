---
title: "Shape.IsHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Indica si el objeto es visible"
type: docs
url: /es/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Indica si el objeto es visible.

```csharp
public bool IsHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Establece la propiedad IsHidden a false (visible)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // Establece la propiedad IsHidden a true (oculto)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


