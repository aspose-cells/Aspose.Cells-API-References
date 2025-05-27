---
title: CommandButtonActiveXControl.PicturePosition
second_title: Aspose.Cells for .NET API Reference
description: CommandButtonActiveXControl property. Gets and set the location of the controls picture relative to its caption
type: docs
url: /net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/
---
## CommandButtonActiveXControl.PicturePosition property

Gets and set the location of the control's picture relative to its caption.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Click Me";
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            
            workbook.Save("CommandButtonWithPicturePosition.xlsx");
        }
    }
}
```

### See Also

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


