---
title: "ImageActiveXControl.SpecialEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl egenskap. Hämtar och anger den speciella effekten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/
---
## ImageActiveXControl.SpecialEffect property

Hämtar och anger den speciella effekten för kontrollen.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Exempel

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

            // Demonstrera egenskapen SpecialEffect
            imageControl.SpecialEffect = ControlSpecialEffectType.Raised;
            
            // Ställ in andra nödvändiga egenskaper
            imageControl.BorderStyle = ControlBorderType.Single;
            byte[] imageData = File.ReadAllBytes("demo.jpg");
            imageControl.Picture = imageData;

            workbook.Save("ImageActiveXControlSpecialEffectDemo.xlsx");
            
            Console.WriteLine($"SpecialEffect set to: {imageControl.SpecialEffect}");
        }
    }
}
```

### Se även

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


