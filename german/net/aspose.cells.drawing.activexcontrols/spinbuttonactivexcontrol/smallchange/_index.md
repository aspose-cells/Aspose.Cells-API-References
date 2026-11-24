---
title: "SpinButtonActiveXControl.SmallChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpinButtonActiveXControl-Eigenschaft. Gibt den Betrag zurück und legt ihn fest, um den sich die Position-Eigenschaft ändert"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/
---
## SpinButtonActiveXControl.SmallChange property

Liest und setzt den Betrag, um den sich die Position‑Eigenschaft ändert

```csharp
public int SmallChange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertySmallChangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein SpinButton-ActiveX-Steuerelement zum Arbeitsblatt hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            
            // Rufen Sie das ActiveX-Steuerelement ab und setzen Sie die SmallChange-Eigenschaft
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.SmallChange = 5;
            
            // Speichere die Arbeitsmappe
            workbook.Save("SpinButtonSmallChangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


