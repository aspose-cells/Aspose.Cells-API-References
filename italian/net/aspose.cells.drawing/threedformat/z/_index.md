---
title: "ThreeDFormat.Z"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Definisce la distanza dal suolo per la forma 3D"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

Definisce la distanza dal suolo per la forma 3D.

```csharp
public double Z { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Accedi al ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore corrente di Z (distanza dal suolo)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Imposta un nuovo valore di Z per spostare la forma più lontano dal suolo
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Configura altre proprietà 3D per rendere visibile l'effetto
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Salva la cartella di lavoro per vedere l'effetto 3D
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


