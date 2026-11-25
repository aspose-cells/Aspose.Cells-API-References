---
title: "ThreeDFormat.Material"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per dare l'aspetto finale di una forma"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Rappresenta il materiale predefinito che viene combinato con le proprietà di illuminazione per fornire l'aspetto finale di una forma.

```csharp
public PresetMaterialType Material { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Accedi al ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visualizza il valore corrente del materiale
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Imposta diversi tipi di materiale e osserva gli effetti
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Configura altre proprietà 3D per vedere meglio l'effetto del materiale
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Salva la cartella di lavoro con gli effetti 3D
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


