---
title: "ShapeSegmentPathCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeSegmentPathCollection-Methode. Fügt einen Segmentpfad im Erstellungsweg hinzu"
type: docs
url: /de/net/aspose.cells.drawing/shapesegmentpathcollection/add/
---
## ShapeSegmentPathCollection.Add method

Fügt einen Segmentpfad zum Erstellungsweg hinzu.

```csharp
public int Add(ShapePathType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ShapePathType | Der Pfadtyp. |

### Rückgabewert

Gibt die Position des [`ShapeSegmentPath`](../../shapesegmentpath/) Objekts in der Liste zurück.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Beginnen Sie einen neuen Pfad
            path.MoveTo(10, 10);

            // Zeichne ein Liniensegment
            path.LineTo(100, 100);

            // Greifen Sie auf die PathSegementList-Eigenschaft zu
            ShapeSegmentPathCollection segmentList = path.PathSegementList;

            segmentList.Add(ShapePathType.Close);

            // Anzahl der Pfadsegmente anzeigen
            Console.WriteLine("Number of path segments: " + segmentList.Count);

            // Durchlaufen Sie jedes Segment und zeigen Sie dessen Typ an
            foreach (ShapeSegmentPath segment in segmentList)
            {
                Console.WriteLine("Segment type: " + segment.Type);
            }

           
            //Freiform hinzufügen
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Speichern Sie die Arbeitsmappe, um die Formänderungen zu beobachten
            workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


