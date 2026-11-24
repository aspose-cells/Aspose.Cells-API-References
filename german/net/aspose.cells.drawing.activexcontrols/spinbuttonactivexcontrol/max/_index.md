---
title: "SpinButtonActiveXControl.Max"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpinButtonActiveXControl-Eigenschaft. Gibt den maximal zulässigen Wert zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Ruft den maximal zulässigen Wert ab und legt ihn fest.

```csharp
public int Max { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein SpinButton-ActiveX-Steuerelement zum Arbeitsblatt hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // Rufen Sie das ActiveX-Steuerelement ab und setzen Sie dessen Max-Eigenschaft
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Speichere die Arbeitsmappe
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


