---
title: "CommandButtonActiveXControl.PicturePosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommandButtonActiveXControl. Obtiene y establece la ubicación de la imagen del control relativa a su caption"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/
---
## CommandButtonActiveXControl.PicturePosition property

Obtiene y establece la ubicación de la imagen del control relativa a su leyenda.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Ejemplos

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

### Ver también

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


