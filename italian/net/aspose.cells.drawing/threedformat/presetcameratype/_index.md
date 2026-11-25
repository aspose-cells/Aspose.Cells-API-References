---
title: "ThreeDFormat.PresetCameraType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta il tipo di telecamera predefinita per l'estrusione"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/presetcameratype/
---
## ThreeDFormat.PresetCameraType property

Ottiene e imposta il tipo di telecamera predefinita per l'estrusione.

```csharp
public PresetCameraType PresetCameraType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPresetCameraTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
            
            // Ottieni il ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore corrente di PresetCameraType
            Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);

            // Imposta un nuovo valore di PresetCameraType
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;

            // Applica una formattazione 3D aggiuntiva per rendere visibile l'effetto
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Visualizza il nuovo valore di PresetCameraType
            Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);

            // Salva la cartella di lavoro per mostrare l'effetto
            workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


