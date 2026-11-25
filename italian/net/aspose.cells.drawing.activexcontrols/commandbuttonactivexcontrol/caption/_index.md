---
title: "CommandButtonActiveXControl.Caption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CommandButtonActiveXControl property. Ottiene e imposta il testo descrittivo che appare su un controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/
---
## CommandButtonActiveXControl.Caption property

Ottiene e imposta il testo descrittivo che appare su un controllo.

```csharp
public string Caption { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl commandButton = (Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl)shape.ActiveXControl;

            // Dimostra l'uso della proprietà Caption
            commandButton.Caption = "Click Me";
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);

            workbook.Save("CommandButtonCaptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


