---
title: "ThreeDFormat.LightingDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta la direzione da cui l'impianto di illuminazione è orientato rispetto alla scena"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/lightingdirection/
---
## ThreeDFormat.LightingDirection property

Ottiene e imposta la direzione da cui l'impianto luminoso è orientato rispetto alla scena.

```csharp
public LightRigDirectionType LightingDirection { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D Lighting Direction Demo";
            
            // Ottieni il ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Imposta le proprietà 3D iniziali
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.Material = PresetMaterialType.Plastic;

            // Visualizza la direzione di illuminazione corrente
            Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);

            // Cambia la direzione di illuminazione e osserva gli effetti
            threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
            Console.WriteLine("Changed LightingDirection to TopLeft");

            // Cambia a un'altra direzione
            threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
            Console.WriteLine("Changed LightingDirection to BottomRight");

            // Salva la cartella di lavoro per vedere gli effetti visivi
            workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


