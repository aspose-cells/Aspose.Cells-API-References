---
title: "ShapeTextAlignment.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment Methode. Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes ShapeTextAlignment-Objekt hat"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes [`ShapeTextAlignment`](../)-Objekt hat.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | Object | Das [`ShapeTextAlignment`](../)-Objekt zum Vergleich mit dieser Instanz. |

### Rückgabewert

true, wenn der Wert des obj-Parameters dem Wert dieser Instanz entspricht; andernfalls false. Wenn obj null ist, gibt diese Methode false zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge eine Form hinzu, um die Textausrichtung zu vergleichen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Hole die Textausrichtung einer anderen Form zum Vergleich
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


