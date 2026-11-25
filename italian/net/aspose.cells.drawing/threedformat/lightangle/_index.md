---
title: "ThreeDFormat.LightAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta l'angolo delle luci di estrusione"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Ottiene e imposta l'angolo delle luci di estrusione.

```csharp
public double LightAngle { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Accedi al ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostra il valore corrente di LightAngle
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Imposta un nuovo valore di LightAngle (da 0 a 359,9 gradi)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // Configura altre proprietà 3D per vedere l'effetto di LightAngle
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


