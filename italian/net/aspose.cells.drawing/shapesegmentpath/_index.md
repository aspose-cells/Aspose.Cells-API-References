---
title: "Classe ShapeSegmentPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ShapeSegmentPath. Rappresenta un percorso di segmento in un percorso della forma libera"
type: docs
url: /it/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Rappresenta un percorso segmento in un percorso del disegno libero.

```csharp
public class ShapeSegmentPath
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Ottiene i punti nel segmento del percorso |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Ottiene il tipo di segmento del percorso |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma libera al foglio di lavoro
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Ottieni il percorso geometrico della forma
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Accedi al primo percorso di segmento (se esiste)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // Dimostra le proprietà di ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Itera attraverso i punti nel percorso del segmento
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


