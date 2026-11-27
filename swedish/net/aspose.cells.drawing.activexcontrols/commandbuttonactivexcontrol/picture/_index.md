---
title: "CommandButtonActiveXControl.Picture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommandButtonActiveXControl-egenskap. Hämtar och anger bildens data"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

Hämtar och anger bildens data.

```csharp
public byte[] Picture { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att hysa ActiveX-kontrollen med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Ställ in egenskaper
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // Ange bilden (tom byte‑array representerar ingen bild)
            button.Picture = new byte[0];

            // Spara arbetsboken
            workbook.Save("CommandButtonWithPicture.xlsx");

            // Verifiera bild‑egenskapen
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### Se även

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


