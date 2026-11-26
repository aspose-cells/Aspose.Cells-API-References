---
title: "Shape.IsSameSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Shape. Devuelve si el shape es idéntico"
type: docs
url: /es/net/aspose.cells.drawing/shape/issamesetting/
---
## Shape.IsSameSetting method

Devuelve si la forma es la misma.

```csharp
public virtual bool IsSameSetting(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape1 = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            if (shape1.IsSameSetting(shape1))
            {
                Console.WriteLine("Same shape object - settings match.");
            }

            if (!shape1.IsSameSetting(shape2))
            {
                Console.WriteLine("Different shape objects - settings don't match.");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


