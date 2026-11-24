---
title: "CommandButtonActiveXControl.Picture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommandButtonActiveXControl-Eigenschaft. Gibt die Bilddaten zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

Liest und setzt die Bilddaten.

```csharp
public byte[] Picture { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form erstellen, um das ActiveX-Steuerelement mit allen erforderlichen Parametern zu hosten
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Eigenschaften festlegen
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // Setzen Sie das Bild (ein leeres Byte-Array steht für kein Bild)
            button.Picture = new byte[0];

            // Speichere die Arbeitsmappe
            workbook.Save("CommandButtonWithPicture.xlsx");

            // Überprüfen Sie die Picture-Eigenschaft
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### Siehe auch

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


