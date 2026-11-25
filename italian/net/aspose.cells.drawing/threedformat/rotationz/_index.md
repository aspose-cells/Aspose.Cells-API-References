---
title: "ThreeDFormat.RotationZ"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta la rotazione della forma estrusa attorno all'asse z in gradi"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Ottiene e imposta la rotazione della forma estrusa attorno all'asse z in gradi.

```csharp
public double RotationZ { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Accedi al ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore corrente di RotationZ
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Imposta nuovi valori di RotationZ e dimostra gli effetti
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Applica altre proprietà 3D per rendere visibile la rotazione
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Salva la cartella di lavoro con gli effetti 3D
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


