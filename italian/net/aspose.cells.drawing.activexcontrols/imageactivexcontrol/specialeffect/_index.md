---
title: "ImageActiveXControl.SpecialEffect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageActiveXControl. Ottiene e imposta l'effetto speciale del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/
---
## ImageActiveXControl.SpecialEffect property

Ottiene e imposta l'effetto speciale del controllo.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Dimostrare la proprietà SpecialEffect
            imageControl.SpecialEffect = ControlSpecialEffectType.Raised;
            
            // Imposta le altre proprietà richieste
            imageControl.BorderStyle = ControlBorderType.Single;
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            workbook.Save("ImageActiveXControlSpecialEffectDemo.xlsx");
            
            Console.WriteLine($"SpecialEffect set to: {imageControl.SpecialEffect}");
        }
    }
}
```

### Vedi anche

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


