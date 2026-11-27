---
title: "CheckBoxActiveXControl.Accelerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl-egenskap. Hämtar och anger acceleratortangenten för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/accelerator/
---
## CheckBoxActiveXControl.Accelerator property

Hämtar och anger acceleratortangenten för kontrollen.

```csharp
public char Accelerator { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl checkBox = (Aspose.Cells.Drawing.ActiveXControls.CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "Check with Alt+A";
            checkBox.Accelerator = 'A';
            checkBox.IsAutoSize = true;

            workbook.Save("CheckBoxAcceleratorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


