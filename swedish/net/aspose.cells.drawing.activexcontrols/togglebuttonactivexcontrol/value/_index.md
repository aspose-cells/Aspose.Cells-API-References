---
title: "ToggleButtonActiveXControl.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Anger om kontrollen är markerad eller inte"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

Anger om kontrollen är markerad eller inte.

```csharp
public CheckValueType Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ToggleButton ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Ange startvärde till Avmarkerad
            toggleButton.Value = CheckValueType.UnChecked;

            // Kontrollera och växla värdet om det är Avmarkerad
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // Spara arbetsboken
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


