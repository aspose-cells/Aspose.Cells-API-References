---
title: "ShapeSegmentPath.Points"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeSegmentPath. Ottiene i punti nel segmento del percorso"
type: docs
url: /it/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Ottiene i punti nel segmento del percorso

```csharp
public ShapePathPointCollection Points { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {// Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Inizia un nuovo percorso
            path.MoveTo(10, 10);

            // Disegna un segmento di linea
            path.LineTo(100, 100);

            // Accedi alla proprietà PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // Accedi al primo percorso del segmento
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Visualizza le informazioni dei punti
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //aggiungi forma libera
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Salva la cartella di lavoro
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


