---
title: "ThreeDFormat.Perspective"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta l'angolo con cui un oggetto ThreeDFormat può essere visualizzato"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Ottiene e imposta l'angolo da cui un oggetto ThreeDFormat può essere visualizzato.

```csharp
public double Perspective { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Ottieni il formato 3D della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostra il valore corrente della prospettiva
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Imposta un nuovo valore di prospettiva (da 0 a 120 gradi)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Applica altri effetti 3D per visualizzare meglio la modifica della prospettiva
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


