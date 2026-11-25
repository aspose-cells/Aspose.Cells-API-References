---
title: "CommandButtonActiveXControl.PicturePosition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CommandButtonActiveXControl property. Ottiene e imposta la posizione dell'immagine del controllo rispetto al suo caption"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/
---
## CommandButtonActiveXControl.PicturePosition property

Ottiene e imposta la posizione dell'immagine del controllo rispetto alla sua didascalia.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Esempi

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

### Vedi anche

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


