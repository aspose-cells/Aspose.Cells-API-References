---
title: "Shape.ToFrontOrBack"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Bringt das Shape nach vorne oder sendet das Shape nach hinten"
type: docs
url: /de/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Bringt die Form nach vorne oder sendet die Form nach hinten.

```csharp
public void ToFrontOrBack(int orders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bestellungen | Int32 | Wenn es kleiner als Null ist, wird das Shape nach hinten gesetzt. Wenn es größer als Null ist, wird das Shape nach vorne gebracht. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie zwei Shapes hinzu, um die Z-Reihenfolge zu demonstrieren
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Verschieben Sie shape2 um 2 Positionen nach vorne in der Z-Reihenfolge
            shape2.ToFrontOrBack(2);

            // Verschieben Sie shape1 um 1 Position nach hinten in der Z-Reihenfolge
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


