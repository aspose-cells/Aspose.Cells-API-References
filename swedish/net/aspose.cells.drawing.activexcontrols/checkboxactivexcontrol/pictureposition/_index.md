---
title: "CheckBoxActiveXControl.PicturePosition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl egenskap. Hämtar och anger platsen för kontrollens bild relativt dess rubrik"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

Hämtar och anger placeringen av kontrollens bild i förhållande till dess rubrik.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX‑kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CheckBox, 
                10,  // left
                10,  // top
                150, // width
                30,  // height
                0,   // leftOffset
                0    // topOffset
            );
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Konfigurera CheckBox‑egenskaperna
            checkBox.Caption = "Sample CheckBox";
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.IsAutoSize = true;

            // Spara arbetsboken
            workbook.Save("CheckBoxPicturePositionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


