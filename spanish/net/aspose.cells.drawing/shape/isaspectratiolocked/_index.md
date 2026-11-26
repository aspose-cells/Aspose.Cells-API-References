---
title: "Shape.IsAspectRatioLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. True indica que la proporción de aspecto de la forma está bloqueada"
type: docs
url: /es/net/aspose.cells.drawing/shape/isaspectratiolocked/
---
## Shape.IsAspectRatioLocked property

True indica que la relación de aspecto de la forma está bloqueada.

```csharp
public bool IsAspectRatioLocked { get; set; }
```

### Observaciones

Solo para imágenes y objetos Ole.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsAspectRatioLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 50);
            
            Console.WriteLine("Original Aspect Ratio Locked: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = true;
            Console.WriteLine("After setting to true: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = false;
            Console.WriteLine("After setting to false: " + shape.IsAspectRatioLocked);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


