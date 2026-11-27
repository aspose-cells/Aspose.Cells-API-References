---
title: "CheckBoxActiveXControl.Caption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl-egenskap. Hämtar och anger den beskrivande texten som visas på en kontroll"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/caption/
---
## CheckBoxActiveXControl.Caption property

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
    public class CheckBoxActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en CheckBox ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Ange och demonstrera Caption-egenskapen
            checkBoxControl.Caption = "Sample CheckBox Caption";
            checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value

            // Spara arbetsboken
            workbook.Save("CheckBoxCaptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


