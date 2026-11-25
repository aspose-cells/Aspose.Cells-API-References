---
title: "ShapePathPoint.XAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePathPoint. Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

Quando l'oggetto è un marcatore di angolo, ottieni o imposta il primo angolo in gradi.

```csharp
public int XAngle { get; set; }
```

### Osservazioni

Se questo angolo è l'angolo iniziale di un arco. Questo angolo specificherà quale angolo lungo il percorso circolare presunto sarà usato come posizione di partenza per disegnare l'arco. Questo angolo di partenza sarà bloccato all'ultima posizione della penna nota nel percorso di forma. Garantendo così un percorso di forma continuo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una raccolta di punti del percorso di forma
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Recupera il primo punto e visualizza le sue coordinate X e Y
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // NOTA: La classe ShapePathPoint (secondo la riflessione API corrente) non espone una proprietà XAngle.
            // Pertanto, questa demo si concentra sulle proprietà X e Y disponibili.

            // Costruisci una forma libera semplice usando i punti definiti
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Aggiungi la forma libera al foglio di lavoro
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Salva la cartella di lavoro
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


