---
title: "CheckBoxActiveXControl.Alignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBoxActiveXControl egenskap. Hämtar och anger positionen för rubriken relativt kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/alignment/
---
## CheckBoxActiveXControl.Alignment property

Hämtar och anger positionen för Caption relativt kontrollen.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            checkBox.Caption = "Sample CheckBox";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            workbook.Save("CheckBoxAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


