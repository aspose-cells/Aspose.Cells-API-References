---
title: "CommandButtonActiveXControl.Caption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommandButtonActiveXControl. Obtiene y establece el texto descriptivo que aparece en un control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/
---
## CommandButtonActiveXControl.Caption property

Obtiene y establece el texto descriptivo que aparece en un control.

```csharp
public string Caption { get; set; }
```

### Ejemplos

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

            // Demuestra el uso de la propiedad Caption
            commandButton.Caption = "Click Me";
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);

            workbook.Save("CommandButtonCaptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


