---
title: "ShapePathPoint.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPoint. Specifica il tipo di valore dell'oggetto corrente"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/type/
---
## ShapePathPoint.Type property

Specifica il tipo di valore dell'oggetto corrente.

```csharp
public ShapePathPointValueType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una shape path point collection
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Aggiungi un punto di coordinata di posizione
                int positionPointIndex = pathPoints.Add(100, 50);
                ShapePathPoint positionPoint = pathPoints[positionPointIndex];

                // Visualizza il valore della proprietà Type per la coordinata di posizione
                Console.WriteLine($"Position Point Type: {positionPoint.Type}");
                Console.WriteLine($"Position Point Type is Position: {positionPoint.Type == ShapePathPointValueType.Position}");

                // Aggiungi un punto marcatore di angolo
                int anglePointIndex = pathPoints.Add(0, 0);
                ShapePathPoint anglePoint = pathPoints[anglePointIndex];
                anglePoint.XAngle = 45;
                anglePoint.YAngle = 90;

                // Visualizza il valore della proprietà Type per il marcatore di angolo
                Console.WriteLine($"Angle Point Type: {anglePoint.Type}");
                Console.WriteLine($"Angle Point Type is Angle: {anglePoint.Type == ShapePathPointValueType.Angle}");

                // Crea un percorso di forma e aggiungi punti
                ShapePath path = new ShapePath();
                path.MoveTo(positionPoint.XPixel, positionPoint.YPixel);
                path.ArcTo(anglePoint.XAngle, anglePoint.YAngle, 100, 100);
                path.Close();

                // Aggiungi forma libera al foglio di lavoro
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Salva la cartella di lavoro
                workbook.Save("ShapePathPointTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [ShapePathPointValueType](../../shapepathpointvaluetype/)
* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


