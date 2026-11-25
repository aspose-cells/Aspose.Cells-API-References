---
title: "ThreeDFormat.Lighting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta il tipo di impianto di illuminazione"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Ottiene e imposta il tipo di impianto luminoso.

```csharp
public LightRigType Lighting { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Ottieni il ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore di illuminazione corrente
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Imposta diversi tipi di illuminazione e osserva gli effetti
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Applica altre proprietà 3D per vedere meglio l'effetto di illuminazione
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // Salva con il primo tipo di illuminazione
            workbook.Save("BrightRoomLighting.xlsx");

            // Cambia a un altro tipo di illuminazione
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Cambia a un terzo tipo di illuminazione
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


