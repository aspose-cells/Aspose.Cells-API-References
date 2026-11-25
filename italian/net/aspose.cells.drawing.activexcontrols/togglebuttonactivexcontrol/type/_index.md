---
title: "ToggleButtonActiveXControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ToggleButtonActiveXControl. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type/
---
## ToggleButtonActiveXControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ToggleButton
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Dimostra l'uso della proprietà Type
            ControlType type = toggleButton.Type;
            Console.WriteLine("Control Type: " + type.ToString());

            // Imposta alcune proprietà
            toggleButton.Caption = "Click Me";
            toggleButton.Value = CheckValueType.Checked;
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


