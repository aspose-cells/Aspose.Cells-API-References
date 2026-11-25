---
title: "ThreeDFormat.RotationY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta la rotazione della forma estrusa attorno all'asse y in gradi"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Ottiene e imposta la rotazione della forma estrusa attorno all'asse y in gradi.

```csharp
public double RotationY { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Accedi al ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore corrente di RotationY
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Imposta nuovi valori di RotationY e dimostra gli effetti
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Applica altre proprietà 3D per rendere visibile l'effetto
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Salva la cartella di lavoro per mostrare gli effetti
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Cambia nuovamente la rotazione e salva un'altra versione
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


