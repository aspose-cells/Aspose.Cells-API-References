---
title: "ToggleButtonActiveXControl.Caption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Ottiene e imposta il testo descrittivo che appare su un controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption/
---
## ToggleButtonActiveXControl.Caption property

Ottiene e imposta il testo descrittivo che appare su un controllo.

```csharp
public string Caption { get; set; }
```

### Esempi

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

### Vedi anche

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


