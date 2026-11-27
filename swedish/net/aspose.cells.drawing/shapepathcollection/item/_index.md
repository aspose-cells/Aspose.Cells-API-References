---
title: "ShapePathCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePathCollection egenskap. Hämtar en skapningsväg"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Hämtar en skapningssökväg.

```csharp
public ShapePath this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Returnerar [`ShapePath`](../../shapepath/) objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePathCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en anpassad form (icke-primitive form) med korrekta parametrar
            Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);

            // Åtkomst till ShapePathCollection
            ShapePathCollection shapePaths = customShape.Paths;

            // Lägg till en ny väg
            int pathIndex = shapePaths.Add();

            // Åtkomst till vägen med Item-egenskap
            ShapePath newPath = shapePaths[pathIndex];

            // Utdatainformation
            Console.WriteLine("Path count: " + shapePaths.Count);
            Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);

            // Spara arbetsboken
            workbook.Save("ShapePathCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


