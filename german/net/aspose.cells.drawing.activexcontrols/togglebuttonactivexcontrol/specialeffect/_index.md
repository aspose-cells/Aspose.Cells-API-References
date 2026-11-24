---
title: "ToggleButtonActiveXControl.SpecialEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ToggleButtonActiveXControl-Eigenschaft. Ruft den Spezialeffekt des Steuerelements ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/specialeffect/
---
## ToggleButtonActiveXControl.SpecialEffect property

Liest und setzt den Spezialeffekt des Steuerelements.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein ToggleButton‑ActiveX‑Steuerelement hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // Die SpecialEffect-Eigenschaft festlegen
            control.SpecialEffect = ControlSpecialEffectType.Bump;

            // Speichere die Arbeitsmappe
            workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


