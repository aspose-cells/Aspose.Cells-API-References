---
title: "SpinButtonActiveXControl.Min"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SpinButtonActiveXControl-Eigenschaft. Liest und schreibt den minimal akzeptablen Wert"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Ruft den minimal zulässigen Wert ab und legt ihn fest.

```csharp
public int Min { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein SpinButton-ActiveX-Steuerelement zum Arbeitsblatt hinzufügen
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Setze die Min-Eigenschaft des SpinButton
            spinButton.Min = 0;
            
            // Setze weitere Eigenschaften, um die Funktionalität zu demonstrieren
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Speichere die Arbeitsmappe
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


