---
title: "CheckBoxActiveXControl.Alignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxActiveXControl-Eigenschaft. Ruft die Position der Beschriftung relativ zum Steuerelement ab und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/alignment/
---
## CheckBoxActiveXControl.Alignment property

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

### Siehe auch

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


