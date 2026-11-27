---
title: "LabelActiveXControl.Caption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LabelActiveXControl egenskap. Hämtar och anger den beskrivande texten som visas på en kontroll"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/caption/
---
## LabelActiveXControl.Caption property

Hämtar och anger den beskrivande texten som visas på en kontroll.

```csharp
public string Caption { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till Label ActiveX Control
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.Label, 0, 0, 0, 0, 100, 30);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Ange och demonstrera Caption-egenskapen
            label.Caption = "Label1aaaa";
            
            // Spara och ladda om för att verifiera beständighet
            string path = "LabelActiveXDemo.xlsm";
            workbook.Save(path, SaveFormat.Xlsm);

            Workbook reopened = new Workbook(path);
            LabelActiveXControl reloadedLabel = (LabelActiveXControl)reopened.Worksheets[0].Shapes[0].ActiveXControl;
            Console.WriteLine("Caption: " + reloadedLabel.Caption);
        }
    }
}
```

### Se även

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


