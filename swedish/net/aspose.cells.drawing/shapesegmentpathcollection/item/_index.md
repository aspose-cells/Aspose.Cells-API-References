---
title: "ShapeSegmentPathCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeSegmentPathCollection-egenskap. Hämtar ShapeSegmentPath-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Hämtar [`ShapeSegmentPath`](../../shapesegmentpath/) objektet.

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Returnerar ett [`ShapeSegmentPath`](../../shapesegmentpath/) objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Starta en ny sökväg
            path.MoveTo(10, 10);

            // Rita ett linjesegment
            path.LineTo(100, 100);

            // Åtkomst till PathSegementList egenskap
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Visa antalet segment i banan
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Demonstrera läsning av Item-egenskapen
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //lägg till fri form
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Spara arbetsboken
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


