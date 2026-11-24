---
title: "ToggleButtonActiveXControl.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ToggleButtonActiveXControl Eigenschaft. Ruft den Typ des ActiveX-Steuerelements ab"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type/
---
## ToggleButtonActiveXControl.Type property

Liest den Typ des ActiveX-Steuerelements.

```csharp
public override ControlType Type { get; }
```

### Beispiele

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

            // Fügen Sie ein ToggleButton‑ActiveX‑Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Demonstriere die Verwendung der Type‑Eigenschaft
            ControlType type = toggleButton.Type;
            Console.WriteLine("Control Type: " + type.ToString());

            // Einige Eigenschaften festlegen
            toggleButton.Caption = "Click Me";
            toggleButton.Value = CheckValueType.Checked;
        }
    }
}
```

### Siehe auch

* enum [ControlType](../../controltype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


