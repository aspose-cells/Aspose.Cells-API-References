---
title: "ShapeSegmentPathCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeSegmentPathCollection-metod. Lägg till en segmentbana i skapandevägen"
type: docs
url: /sv/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Lägg till en segmentväg i skapandevägen.

```csharp
public int Add(ShapePathType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ShapePathType | Sökvägstypen. |

### Returvärde

Returnerar positionen för [`ShapeSegmentPath`](../../shapesegmentpath/) objektet i listan.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
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
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Visa antalet segment i banan
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Iterera genom varje segment och visa dess typ
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //lägg till fri form
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Spara arbetsboken för att observera formmodifieringarna.
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


