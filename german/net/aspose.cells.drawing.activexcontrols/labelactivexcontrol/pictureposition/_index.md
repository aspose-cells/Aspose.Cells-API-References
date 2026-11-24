---
title: "LabelActiveXControl.PicturePosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LabelActiveXControl-Eigenschaft. Liest und schreibt die Position des Bildes des Steuerelements relativ zu seiner Beschriftung"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/pictureposition/
---
## LabelActiveXControl.PicturePosition property

Liest und setzt den Ort des Bildes des Steuerelements relativ zu seiner Beschriftung.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


