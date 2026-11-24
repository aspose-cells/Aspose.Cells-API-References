---
title: "Shape.IsSameSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt zurück, ob das shape gleich ist"
type: docs
url: /de/net/aspose.cells.drawing/shape/issamesetting/
---
## Shape.IsSameSetting method

Gibt zurück, ob die Form gleich ist.

```csharp
public virtual bool IsSameSetting(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object |  |

### Beispiele

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

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


