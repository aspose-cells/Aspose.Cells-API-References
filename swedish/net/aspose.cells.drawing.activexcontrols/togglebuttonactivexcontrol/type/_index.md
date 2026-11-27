---
title: "ToggleButtonActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ToggleButtonActiveXControl-egenskap. Hämtar typen av ActiveX‑kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type/
---
## ToggleButtonActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

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

            // Lägg till en ToggleButton ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Demonstrera användning av Type-egenskapen
            ControlType type = toggleButton.Type;
            Console.WriteLine("Control Type: " + type.ToString());

            // Ställ in några egenskaper
            toggleButton.Caption = "Click Me";
            toggleButton.Value = CheckValueType.Checked;
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


