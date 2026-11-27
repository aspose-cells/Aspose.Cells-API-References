---
title: "ShapeTextAlignment.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-metod. Avgör om detta objekt har samma värde som ett annat specificerat ShapeTextAlignment-objekt"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Avgör om detta objekt har samma värde som ett annat specificerat [`ShapeTextAlignment`](../)-objekt.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Det [`ShapeTextAlignment`](../)-objektet att jämföra med denna instans. |

### Returvärde

Sant om värdet på parametern obj är detsamma som värdet på detta objekt; annars falskt. Om obj är null returnerar denna metod falskt.

### Exempel

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
            
            // Lägg till en form för att jämföra textjustering
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Hämta en annan figurs textjustering för jämförelse
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

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


