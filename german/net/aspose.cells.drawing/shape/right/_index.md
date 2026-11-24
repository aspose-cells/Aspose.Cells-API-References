---
title: "Shape.Right"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Breite des horizontalen Versatzes des Shapes von seiner unteren rechten Eckspalte in Pixeln an"
type: docs
url: /de/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Stellt die Breite des horizontalen Versatzes der Form von ihrer unteren rechten Eckspalte dar, in Pixeln.

```csharp
public int Right { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Setzen und lesen Sie die Right-Eigenschaft
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Ändern Sie die Right-Eigenschaft bedingt
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


