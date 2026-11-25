---
title: "ShapePathPoint.YAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPoint. Quando l'oggetto è un indicatore di angolo, ottieni o imposta il secondo angolo in gradi"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

Quando l'oggetto è un marcatore di angolo, ottieni o imposta il secondo angolo in gradi.

```csharp
public int YAngle { get; set; }
```

### Osservazioni

Se questo angolo è l'angolo di swing di un arco. Questo angolo specificherà quanto, in termini di angolo, lungo il percorso circolare presunto, l'arco sarà esteso. L'estensione dall'angolo iniziale sarà sempre nella direzione oraria attorno al cerchio presunto.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
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

                // Aggiungi punti con indicatori di angolo (usando XAngle e YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Visualizza il valore di YAngle
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Crea un altro punto con angoli diversi
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Visualizza il valore di YAngle
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Crea un percorso di forma e aggiungi un arco usando i marcatori di angolo
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

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
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


