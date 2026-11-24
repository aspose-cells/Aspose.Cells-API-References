---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RadioButtonActiveXControl Eigenschaft. Liest und setzt die Position der Beschriftung relativ zum Steuerelement"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Liest und setzt die Position der Caption relativ zum Steuerelement.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie eine neue Formsammlung und fügen Sie ein ActiveX-Steuerelement hinzu
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Setzen Sie die Alignment-Eigenschaft
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Speichere die Arbeitsmappe
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


