---
title: "LabelActiveXControl.PicturePosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl egenskap. Hämtar och anger placeringen av kontrollens bild i förhållande till dess rubrik"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/pictureposition/
---
## LabelActiveXControl.PicturePosition property

Hämtar och anger placeringen av kontrollens bild i förhållande till dess rubrik.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Demo Label";
            label.PicturePosition = ControlPicturePositionType.AboveLeft;
            
            Console.WriteLine("Label Picture Position: " + label.PicturePosition);
            
            workbook.Save("LabelActiveXControlPicturePositionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


