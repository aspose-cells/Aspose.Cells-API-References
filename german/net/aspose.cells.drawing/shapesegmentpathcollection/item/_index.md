---
title: "ShapeSegmentPathCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeSegmentPathCollection-Eigenschaft. Gibt das ShapeSegmentPath-Objekt zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapesegmentpathcollection/item/
---
## ShapeSegmentPathCollection indexer

Ruft das [`ShapeSegmentPath`](../../shapesegmentpath/) Objekt ab.

```csharp
public ShapeSegmentPath this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Gibt ein [`ShapeSegmentPath`](../../shapesegmentpath/) Objekt zurück.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Beginnen Sie einen neuen Pfad
            path.MoveTo(10, 10);

            // Zeichne ein Liniensegment
            path.LineTo(100, 100);

            // Greifen Sie auf die PathSegementList-Eigenschaft zu
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;


            segmentPaths.Add(ShapePathType.Close);

            // Anzahl der Pfadsegmente anzeigen
            Console.WriteLine("Number of path segments: " + segmentPaths.Count);
          
            
            // Demonstriere das Lesen der Item-Eigenschaft
            for (int i = 0; i < segmentPaths.Count; i++)
            {
                ShapeSegmentPath segment = segmentPaths[i];
                Console.WriteLine($"Segment {i} type: {segment.Type}");
            }

            //Freiform hinzufügen
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


