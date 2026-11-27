---
title: "ImageActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageActiveXControl-egenskap. Hämtar typen av ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/
---
## ImageActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en Image ActiveX Control
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 1, 1, 200, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
            
            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Control Type: " + imageControl.Type);
            
            // Ställ in några egenskaper
            imageControl.IsAutoSize = false;
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Clip;
            
            // Spara arbetsboken
            workbook.Save("ImageActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


