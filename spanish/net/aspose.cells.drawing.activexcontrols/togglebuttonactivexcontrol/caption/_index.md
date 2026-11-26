---
title: "ToggleButtonActiveXControl.Caption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ToggleButtonActiveXControl. Obtiene y establece el texto descriptivo que aparece en un control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption/
---
## ToggleButtonActiveXControl.Caption property

Obtiene y establece el texto descriptivo que aparece en un control.

```csharp
public string Caption { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 2, 0, 2, 0, 100, 30);
            ToggleButtonActiveXControl toggleButtonControl = (ToggleButtonActiveXControl)shape.ActiveXControl;
            toggleButtonControl.Caption = "ExampleButton";

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


