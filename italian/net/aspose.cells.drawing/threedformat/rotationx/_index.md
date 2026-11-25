---
title: "ThreeDFormat.RotationX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta la rotazione della forma estrusa attorno all'asse x in gradi"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Ottiene e imposta la rotazione della forma estrusa attorno all'asse x in gradi.

```csharp
public double RotationX { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // Ottieni il formato 3D (non è necessario "abilitare" gli effetti 3D - basta impostare le proprietà)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore corrente di RotationX
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Imposta un nuovo valore di RotationX (rotazione attorno all'asse x in gradi)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Imposta altre proprietà 3D per rendere visibile la rotazione
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


